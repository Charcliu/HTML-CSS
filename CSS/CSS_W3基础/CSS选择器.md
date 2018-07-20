### id选择器

-   id 选择器可以为标有特定 id 的 HTML 元素指定特定的样式。
    id 选择器以 "#" 来定义。

-   > \#red {color:red;}
    > \#green {color:green;}

### 类选择器

-   类选择器以一个点号显示：

-   > .center {text-align: center}

### 属性选择器

-   对带有指定属性的 HTML 元素设置样式。

````
  [attribute]	用于选取带有指定属性的元素。
  [attribute=value]	用于选取带有指定属性和值的元素。
  [attribute~=value]	用于选取属性值中包含指定词汇的元素。
  [attribute|=value]	用于选取带有以指定值开头的属性值的元素，该值必须是整个单词。
  [attribute^=value]	匹配属性值以指定值开头的每个元素。
  [attribute$=value]	匹配属性值以指定值结尾的每个元素。
  [attribute*=value]	匹配属性值中包含指定值的每个元素。
````

-   > [title]{
    > border:5px solid blue;
    > }

### 元素选择器

- 元素就是最基本的选择器。

-   > html {color:black;}
    > h1 {color:blue;}
    > h2 {color:silver;}

### 选择器分组

-   > ** no grouping **

-   > h1 {color:blue;}
    > h2 {color:blue;}
    > h3 {color:blue;}
    > h4 {color:blue;}
    > h5 {color:blue;}
    > h6 {color:blue;}

-   > ** grouping **

-   > h1, h2, h3, h4, h5, h6 {color:blue;}

### 后代选择器

-   后代选择器（descendant selector）又称为包含选择器。
    后代选择器可以选择作为某元素后代的元素。
-   > h1 em {color:red;}

  >  ````
    派生选择器
    通过依据元素在其位置的上下文关系来定义样式，你可以使标记更加简洁。
    li strong {
       font-style: italic;
        font-weight: normal;
    }
````

### 子元素选择器

-   子元素选择器（Child selectors）只能选择作为某元素子元素的元素。
-   > h1 > strong {color:red;}

### 相邻兄弟选择器

-   相邻兄弟选择器（Adjacent sibling selector）可选择紧接在另一元素后的元素，且二者有相同父元素。
-   >  h1 + p {margin-top:50px;}

### CSS伪类

- CSS 伪类用于向某些选择器添加特殊的效果。

- ###### 锚伪类
> 在支持 CSS 的浏览器中，链接的不同状态都可以不同的方式显示，这些状态包括：活动状态，已被访问状态，未被访问状态，和鼠标悬停状态。

  ````
  a:link {color: #FF0000}		/* 未访问的链接 */
  a:visited {color: #00FF00}	/* 已访问的链接 */
  a:hover {color: #FF00FF}	/* 鼠标移动到链接上 */
  a:active {color: #0000FF}	/* 选定的链接 */
  ````

| 属性           |           描述          | CSS |
| ------------ | :-------------------: | --: |
| :active      |      向被激活的元素添加样式。     |   1 |
| :focus       |   向拥有键盘输入焦点的元素添加样式。   |   2 |
| :hover       |  当鼠标悬浮在元素上方时，向元素添加样式。 |   1 |
| :link        |     向未被访问的链接添加样式。     |   1 |
| :visited     |     向已被访问的链接添加样式。     |   1 |
| :first-child |    向元素的第一个子元素添加样式。    |   2 |
| :lang        | 向带有指定 lang 属性的元素添加样式。 |   2 |

### CSS伪元素
-   ###### :before 伪元素
    >  ":before" 伪元素可以在元素的内容前面插入新内容。

    ````

      h1:before
      {
        content:url(logo.gif);
      }

    ````

-   ######     :after 伪元素
   > ":after" 伪元素可以在元素的内容之后插入新内容。

   ````

    h1:after
     {
       content:url(logo.gif);
     }

  ````
