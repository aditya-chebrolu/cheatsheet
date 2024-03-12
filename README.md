# cheatsheet

* [DEVTOOLS](#devtools)
* [CSS](#css)
* [BASH](#bash)


## DEVTOOLS

```$$('div')``` - querySelectorAll

```$('div')``` - querySelector

```$_``` - Result of last operation

## CSS
No Scroll bar
```
::-webkit-scrollbar {
    display: none;
}
```

Remove type="number"the arrow at the end
```
input::-webkit-outer-spin-button,
input::-webkit-inner-spin-button {
   -webkit-appearance: none;
}
```
Line clamp
```
display: -webkit-box;
-webkit-line-clamp: 3;
-webkit-box-orient: vertical;  
overflow: hidden;
```
Full bleed
```
box-shadow: 0 0 0 1000vmax black;
clip-path: inset(0 -100vmax);
```
Transition to heigh auto
```
.wrapper {
   display:grid;
   grid-template-rows:0fr;
   transition: grid-template-rows 0.5s;
}
.wrapper.is-open {
   grid-template-rows: 1fr;
}
.inner {
   overflow:hidden;
}
```

Note:
- apply overflow to flex-item might shrink it.

  fix: `flex-shrink:0`

 ## BASH
 Set an alias
 
```
alias key='value'
```
list of currently set env. variables
```
printenv
```
```
env
```
Get the value of the variable
```
$<variable_name>
```
Set temp. env. variable
```
export PATH=/Users/test/test_folder:$PATH
```
Set permanent env. variable
```
nano ~/.zshrc
```
```
export <var>=<value>
```
Unset env. variable
```
unset <key>
```
Location of a package
```
which <package_name>
```
