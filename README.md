# CSS: Selectors

![image](https://github.com/luiscoco/CSS_Selectors/assets/32194879/88bf930a-ff76-415f-ab42-daca885b6972)

## 1. The CSS element Selector

Here, all ```<p>``` elements on the page will be center-aligned, with a red text color: 

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

## 2. The CSS id Selector

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

## 3. The CSS class Selector

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

In this example only ```<p>``` elements with class="center" will be red and center-aligned: 

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    p.center {
      text-align: center;
      color: red;
    }
    </style>
  </head>
  <body>
    <h1 class="center">This heading will not be affected</h1>
    <p class="center">This paragraph will be red and center-aligned.</p> 
  </body>
</html>
```

In this example the ```<p>``` element will be styled according to class="center" and to class="large": 

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    p.center {
      text-align: center;
      color: red;
    }
    
    p.large {
      font-size: 300%;
    }
    </style>
  </head>
  <body>
    <h1 class="center">This heading will not be affected</h1>
    <p class="center">This paragraph will be red and center-aligned.</p>
    <p class="center large">This paragraph will be red, center-aligned, and in a large font-size.</p> 
  </body>
</html>
```

## 4. The CSS Universal Selector

The universal selector (*) selects all HTML elements on the page.

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    * {
      text-align: center;
      color: blue;
    }
    </style>
  </head>
  <body>
    <h1>Hello world!</h1>
    <p>Every element on the page will be affected by the style.</p>
    <p id="para1">Me too!</p>
    <p>And me!</p>
  </body>
</html>
```

## 5. The CSS Grouping Selector

The grouping selector selects all the HTML elements with the same style definitions.

Look at the following CSS code (the h1, h2, and p elements have the same style definitions):

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
    h1, h2, p {
      text-align: center;
      color: red;
    }
    </style>
  </head>
  <body>
    <h1>Hello World!</h1>
    <h2>Smaller heading!</h2>
    <p>This is a paragraph.</p>
  </body>
</html>
```



