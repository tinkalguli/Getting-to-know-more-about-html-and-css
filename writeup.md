# Getting to Know More About HTML-CSS


## Semantic code :

Semantic means using a proper element for appropriate content.
for example :

We  have to use `h1` element for a main heading .(Which is used once in a page)

```
<h1>THIS IS THE MAIN HEADING</h1>
```
## Block and inline level element

Block level element take the whole width of a page or display and begin from a new line.
Inline level element take the width according to the content and does not start in a new line.

## Text Based Elements

Some deferent types of text based element are headings(h1...h6), p, strong , bold , em , i etc.

## Creating Hyperlinks

We have two types of hyperlink's path :
* Relative path
* Absolute path

### Relative path

If the link connects to the other pages of the same website then it is considered as a relative path.

```
 <a href="about.html">About</a>
```

### Absolute path

If the link connects to another website which is entirely different from the current one, then it is considered to have an absolute path.

```
<a href="https://www.google.com/">Google</a>
```

* Linking to Email Address

To create a email hyperlink "href" attribute value includes mailto: followed by the email address. For example:

```
<a href="mailto:xyz@example.com?subject=Reaching%20Out&body=How%20are%20you?">Mail Me</a>
```

## Structure Based Elements

Some of structure based elements are <header>, <nav>, <section>, <article>, <aside>, and <footer>.

![Structure](https://raw.githubusercontent.com/suraj122/AC-STYLE-images/master/html-css/Structure.png)


## CSS Resets

CSS resets takes all the element and provides unified styles for all browser. It removes all the default sizing, margin, padding, and all the additional styles from the element.

[ Eric Meyer’s reset ](https://meyerweb.com/eric/tools/css/reset/)

```
/* http://meyerweb.com/eric/tools/css/reset/
 v2.0 | 20110126
 License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header, hgroup,
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure,
footer, header, hgroup, menu, nav, section {
  display: block;
}
body {
  line-height: 1;
}
ol, ul {
  list-style: none;
}
blockquote, q {
  quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
  content: '';
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
```

## The Cascading Rule

CSS is a "Cascading Style Sheet" where styles cascade from top to bottom. Cascading allows to add different styles and overwrite the previous styles. In cascading whatever styles come at the bottom will have more precedence than the earlier one. For example:

```
p{
  color: red;
}
p{
  color: green;
}
```
In the above example the green color will be applied in the paragraph .

## Specificity weight of selectors

* Type: 0-0-1
* Class: 0-1-0
* ID: 1-0-0

```
<p class="para" id="paragraph">

#paragraph{
  background: red;
}
.para{
  background: green;
}
p{
  background: blue;
}
```

In the above example the red color with id="paragraph" will be applied to the paragraph because specificity of id selectors is more than the type and class selector.

## Common CSS Property & Values

### color

Values of the color property are in keywords(black,white etc.),rgb values(rgb(255,40,0)etc.),hex values(#fff,#56af3a etc), hsl values (hls(24,100%,50%)etc.).

### length

We have absolute lengths e.i. pixels (px)etc. we have relative lengths percentage(%),em, etc.
