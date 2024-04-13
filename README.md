# CSS: Selectors

**The CSS element Selector**

Here, all <p> elements on the page will be center-aligned, with a red text color: 

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    p {
      text-align: center;
      color: red;
    } 
    </style>
  </head>
  <body>
    <p>Every paragraph will be affected by the style.</p>
    <p id="para1">Me too!</p>
    <p>And me!</p>
  </body>
</html>
```
**The CSS id Selector**

The CSS rule below will be applied to the HTML element with id="para1": 

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    #para1 {
      text-align: center;
      color: red;
    }
    </style>
  </head>
  <body>
    <p id="para1">Hello World!</p>
    <p>This paragraph is not affected by the style.</p>
  </body>
</html>
```

**The CSS class Selector**

In this example all HTML elements with class="center" will be red and center-aligned: 

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    .center {
      text-align: center;
      color: red;
    }
    </style>
  </head>
  <body>
    <h1 class="center">Red and center-aligned heading</h1>
    <p class="center">Red and center-aligned paragraph.</p> 
  </body>
</html>
```



