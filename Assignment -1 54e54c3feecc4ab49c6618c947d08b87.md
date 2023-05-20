# Assignment -1


# scss

Officially described as “[CSS with superpowers](https://sass-lang.com/),”  SCSS (or Sass) offers a way to write styles for websites with more enhanced CSS syntax

for example

```
body {
  background-color:#000;
  color:#fff;
}
```

SCSS allows us to nest selectors that repeat the same root text

```
.header {
  width: 50%;
  margin: 0 auto;

  &-link {
    color: blue;
  }
}
```

# Bootstrap

Bootstrap is a free,open source front-end development framework for the creation of websites and web apps. It is designed for developing a responsive websites. It provides a collection of syntax for template designs.

A website is called responsive website which can automatically adjust itself to look good on all devices, from smart phones to desktops etc.

**what bootstrap package contains**

**scafffolding**:Bootstrap provides a basic structure with Grid system , link styles and background.

**css**:Bootstrap comes with the feature of global css settings,fundamental HTML elements style and an advanced grid system. grid system has two container classes to better accomodate both deskop and mobile-based projects-a fixed container(.container) and a fluid container(.container-fluid). The first container class provides a fixed-width container , while the second offers a full-width container capable of adjusting your project to all screen sizes.

**components**: bootsrap contains a lot of reusable components built to provide iconography,dropdowns,navigation,alerts,pop-overs and much more.

**customize**:Bootstrap components are customizable and you can customize bootstrap’s components.

for example we can see the grid system

# css

CSS (Cascading Style Sheets) allows you to create great-looking web pages.

CSS is a rule-based language — you define the rules by specifying groups of styles that should be applied to particular elements or groups of elements on your web page.

CSS can be added to HTML documents in 3 ways

- **Inline** - by using the style attribute inside HTML elements
- **Internal** - by using a <style> element in the <head> section
- **External** - by using a <link> element to link to an external CSS file

CSS consists of two components:

- **Properties**: These are human-readable identifiers that indicate which stylistic features you want to modify. For example, `[font-size](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)`, `[width](https://developer.mozilla.org/en-US/docs/Web/CSS/width)`, `[background-color](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)`.
- **Values**: Each property is assigned a value. This value indicates how to style the property.

CSS properties and values are case-insensitive. The property and value in a property-value pair are separated by a colon (`:`).

# css tags

- `color` property for text colors
- `font-family` property for text fonts
- `font-size` property for text sizes
- `border` property for borders
- `padding` property for space inside the border
- `margin` property for space outside the border

# HTML tags

Represent six levels of section headings. `<h1>` is the highest section level and `<h6>` is the lowest.

<li> used to list items

<ul> used to list unorderly

<ol> used to list ordered list

<i> used to write in italics

<img>Embeds an image into the document.

<video>Embeds an image into the document.

<link>Defines the relationship between a document and an external resource (most used to link to style sheets)

<p> Defines a paragraph

<select> Defines a drop-down list

<audio> Defines sound content

# Pseudoclass seletor

A  **css** ***pseudo-class*** is a keyword added to a selector that specifies a special state of the selected element(s). For example, the pseudo-class `[:hover](https://developer.mozilla.org/en-US/docs/Web/CSS/:hover)` can be used to select a button when a user's pointer hovers over the button and this selected button can then be styled.

# pseudo element

A CSS pseudo-element is used to style specified parts of an elemen

For example, it can be used to:

- Style the first letter, or line, of an element
- Insert content before, or after, the content of an element

# Attribute selector

**CSS** attribute selector is a type of selector that ****selects HTML elements based on their attributes or attribute values.

-The `[attribute]` selector is used to select elements with a specified attribute.

 The following example selects all <a> elements with a target attribute:

a[target] {

background-color: yellow;

}

-The `[attribute$="value"]` selector is used to select elements whose attribute value ends with a specified value.

-The `[attribute*="value"]` selector is used to select elements whose attribute value contains a specified value.

# Combinator selector

It means that the combination of two selectors with the help of some operators or symbols like greater than (>), plus (+), tilde (~).

A CSS selector can contain more than one simple selector. Between the simple selectors, we can include a combinator.

There are four different combinators in CSS:

- descendant selector (space)-The descendant selector matches all elements that are descendants of a specified element.
- child selector (>)-The child selector selects all elements that are the children of a specified element.
- adjacent sibling selector (+)-The adjacent sibling selector is used to select an element that is directly after another specific element.
- general sibling selector (~)-The general sibling selector selects all elements that are next siblings of a specified element.

# Simple selector

Selectors allow you to target and select specific parts of your document for styling purposes.

1.universal selector: selects every single element. use the astericks character to use universal selector.

2.Type selector: selects all html elements of specific types.

3.class selector selects html elements based on the value of their given class. With class selector you can select multiple elements at a times. use dot(.) character followed by the class name.

[4.ID](http://4.ID) selector: selects a html element based on the value of id. Use the(#) character followed by the name of the id value

# XML

- XML stands for eXtensible Markup Language
- XML is a markup language much like HTML
- XML was designed to store and transport data

XML and HTML were designed with different goals:

- XML was designed to carry data - with focus on what data is
- HTML was designed to display data - with focus on how data looks
- XML tags are not predefined like HTML tags are, you can define your own tag in XML.
