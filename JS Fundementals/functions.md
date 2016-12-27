## Function essentials

1. This is a function declaration
    ```
    function fun(){
      console.log("hello");
    }
    ```
2. A function's signature is it's order of parameters or variables
    ```
    function fun(p1){
      return p1+"!!!";
    }
    ```
3. Function expressions are functions stored in variables. In this case myfunc is the name of the variable in which the function is stored and not the function name itself. This is an anonymous function.
  - This is an anonymous function expression:
    ```
    var myfunc=function(){
      return "yo!";
    }
    ```
  - This is a named function expression (used to prevent function hoisting):
    ```
    var myfunc=function myfunc(){
      return "yo!";
    }
    ```
  - IIAF (iffy)
    ```
    (function fun(){
      return "this was invoked automatically"
    }());
    ```
  - Unary function - ASI (automatic semicolon insertion)
    ```
    !function alsoInvokeAutomatically(){
      return "also invoked automatically"
    }
    ```

## Function scope

Scope defines the visibility of our variables in our code.

  - Global scope is the window object
  ```
  window.nameofglobalvariable
  window.location.href
  ```
  - JS has a concept called Function Scope
    - all variables declared in that function are local to that function
    - they cannot be accessed outside the function
    - Use an immediately invoked function to create a local scope for your code

## The this keyword

  - usually a object
  - strict mode
  'use strict' in the first line of our javascript
    ```
    (function(){
      'use strict';
      }());
    ```
  - 
