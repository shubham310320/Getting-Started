# <p style="text-align:center">**HTML**</p>

### **HTML** stands for **H**_yper_ **T**_ext_ **M**_arkup_ **L**_anguage_.

### It is not a programming language it is a **Markup language**.

---

## **HTML Document Structure**

An HTML document structure looks like this:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title></title>
    <meta charset="UTF-8" />
  </head>

  <body>
    all the content that will be displayed on the webpage is written here with
    the use of tags
  </body>
</html>
```

---

## **Text Elements**

> There are total of 6 different types of headings in an html document that are :

```html
<h1>Heading1</h1>

<h2>Heading2</h2>

<h3>Heading3</h3>

<h4>Heading4</h4>

<h5>Heading5</h5>

<h6>Heading6</h6>
```

> Paragraphs are defined by :

```html
<p>This is a paragraph</p>
```

> Lists can be defined by :

```html
<ol class="this is an Ordered list">
  <li>These are the TAGS used for the list items.</li>
</ol>

<ul class="this is an Unordered list">
  <li>These are the TAGS used for the list items.</li>
</ul>
```

> Tables are defined as :

```html
<table>
  <tr class="Table Row">
    <th class="Table Heading">Name</th>
    <th class="Table Heading">Contact</th>
    <th class="Table Heading">Country</th>
  </tr>
  <tr class="Table Row">
    <td class="Tabel Cell">Shubham</td>
    <td class="Tabel Cell">8120120986</td>
    <td class="Tabel Cell">India</td>
  </tr>
  <tr class="Table Row">
    <td class="Tabel Cell">Khushi</td>
    <td class="Tabel Cell">7724019916</td>
    <td class="Tabel Cell">India</td>
  </tr>
</table>
```

---

## **Images and Attributes**

> Images can be added by the tag:

```html
<img
  src="here we can write the destination URL of the image with its proper      directory location for eg. images/image.jpg"
  alt="here comes the text that will be displayed in place of the image if its unable to be loaded."
  width="here comes the width of image"
  hieght="here comes the hieght of image"
/>
```

#### **This tag does not have a closing tag instead it uses _ATTRIBUTES_ {SRC,WIDTH,ALT,HEIGHT etc.} to define the details of its content.**

---

## **Hyperlinks**

> The links on a page leading to any other webpage or a page in the website itself are inserted using the HYPERLINKS:

```html
<a href="URL of the webpage" target="\_blank">This is a link</a>
```

#### **The "target" attribute tells to open the link in a new tab.**

#### **We can add a ' # ' to the " href " attribute to link nowhere. This leads to the top of the page.**

---

## **Structuring a webpage**

#### There are Some container tags used to structure the page with some Semantic meaning to its content Such as:-

> This is a **Header Tag**

```html
<header>This is to define the header part of any section in our page.</header>
```

> This is a **Navigation Tag**

```html
<nav>This is used to define the navigation area on a page.</nav>
```

> This is a **Article Tag**

```html
<article>
  This is used to define the Main content on a page, mostly on blogspot type of
  webpages.
</article>
```

> This is a **Aside Tag**

```html
<aside>
  This is used to define the sider contents or the contents in a sidebar.
</aside>
```

> This is a **Div Tag**

```html
<div>
  This is used to contain contents without any semantic meaning. It is just used
  as a container for the contents.
</div>
```

> This is a **Footer Tag**

```html
<footer>
  This is used for the information that is in the last of a page such as contact
  and copyright disclaimers.
</footer>
```
