### CSS引入的三种方式

- 外部样式表

````
    <head>
      <link rel="stylesheet" type="text/css" href="mystyle.css" />
    </head>
````

- 内部样式表

````
    <head>
      <style type="text/css">
        hr {color: sienna;}
        p {margin-left: 20px;}
        body {background-image: url("images/back40.gif");}
      </style>
    </head>
````

- 内联样式

````
    <p style="color: sienna; margin-left: 20px">
      This is a paragraph
    </p>

````
