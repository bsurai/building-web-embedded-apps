# building-web-embedded-apps
How to build nice embedded app for web

ROOT ELEMENT

Html elements of your app can inherit some styles from host site. You should use `all: initial` rule to avoid it.
#your-root-selector {
  all: inherit;
}


DEPRECATED TAGS

They are:

h1, h2, h3...
a,
p,
i,
button,
ul, li.

Avoid these tags if you can. Because developers of host sites like to use css selectors by them with no classes:
a {...}
p {...}
Css rules like above can add some styles to your elements.


APPROVED TAGS

Instead use tags:

div - for block and flexbox elements

span - for inline elements

These tags usually are styled via classes and indexes. Therefore chances to get conflict with css are very low.


TAGS REPLACEMENT

h1, h2..., i - span

a - span or div. Depends on you need either inline or block element. Moving to another page (url in href) can be implemented via java script code.

p, button, ul, li - use div tag.
