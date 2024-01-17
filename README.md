# cheatsheet

* [DEVTOOLS](#devtools)
* [CSS](#css)


## DEVTOOLS

```$$('div')``` - querySelectorAll

```$('div')``` - querySelector

```$_``` - Result of last operation

## CSS
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


