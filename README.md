# cheatsheet

* [DEVTOOLS](#devtools)
* [CSS](#css)
* [BASH](#bash)
* [BREW](#brew)


## DEVTOOLS

```$$('div')``` - querySelectorAll

```$('div')``` - querySelector

```$_``` - Result of last operation

## BREW
```brew list --cask```

```brew list --formula```

## CSS
1. **No Scroll bar**
   ```css
   ::-webkit-scrollbar {
    display: none;
   }
   ```

2. **Remove type="number"the arrow at the end**
    ```css
    input::-webkit-outer-spin-button,
    input::-webkit-inner-spin-button {
       -webkit-appearance: none;
    }
    ```
3. **Line clamp**
    ```css
    display: -webkit-box;
    -webkit-line-clamp: 3;
    -webkit-box-orient: vertical;  
    overflow: hidden;
    ```
4. **Full bleed**
    ```css
    box-shadow: 0 0 0 1000vmax black;
    clip-path: inset(0 -100vmax);
    ```
5. **Transition to heigh auto**
    ```css
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

6. **fade gradient**
   ```css
   background: linear-gradient(to bottom, rgba(255, 255, 255, 0), rgba(0, 0, 0, 1));
   ```


Note:
- apply overflow to flex-item might shrink it.

  fix: `flex-shrink:0`

 ## BASH
 1. **Set an alias**
    ```
    alias key='value'
    ```
    
2. **Location of a package**
    ```
    which <package_name>
    ```
    
3. **[set | unset variables](https://phoenixnap.com/kb/set-environment-variable-mac)**

