---
title: Document Object Model
type: lesson
duration: 1
authors:
    creators: Jesse Shawl (DC)
    editors: John Master (DC), Matt Scilipoti (DC)
competencies: Programming, Javascript
---

# DOM

- Explain what the DOM is and how it is structured
- Select and target DOM elements using DOM methods
- Select and target DOM elements using a query selector
- Create, read, update, and delete DOM elements
- Change the attributes or content of a DOM element

## Document Object Model (5 min)

The [**D**ocument **O**bject **M**odel](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
is a programming interface for HTML.

An HTML *document* is available for us to manipulate as an object, and this object is structured like a tree:

(Not like this one http://hakim.se/experiments/css/domtree/)

More like this:

![](http://www.tuxradar.com/files/LXF118.tut_grease.diagram.png)

Or this:

html
  |- header
  |- body
      |- h1

## Accessing the document (10 min)

`document`
  - `document.head`
  - `document.body`

Each web page loaded in the browser has its own document object. The Document interface serves as an entry point to the web page's content

### Element attributes

`document.body`
  - .children
  - .childNodes
  - .firstChild
  - .lastChild
  - .nextSibling
  - .parentElement
  - .parentNode

Methods are available on any element.

### Methods for selecting elements

- document.getElementById
- document.getElementsByTagName
- document.getElementsByClassName
- document.querySelector
- document.querySelectorAll

## You Do: Selecting DOM elements (10 min)



## Altering DOM Elements (5 min)

- .textContent
- .innerHTML
- .setAttribute(name, value);
- .id
- .classList.toggle (add, remove, contains)
- .style

## You do: Logo hijack (10 min)

- Open up www.google.com in Chrome or Firefox, and open up the console.
- Find the Google logo and store it in a variable.
- Modify the source of the logo IMG so that it's a Yahoo logo instead.
- Find the Google search button and store it in a variable.
- Modify the text of the button so that it says "Yahooo!" instead.

Bonus: ???


## You Do: Creating/Removing DOM Elements (15 min)

- .createElement
- .appendChild
- .removeChild

## Break (5 min)

## Events (10 min)

- https://developer.mozilla.org/en-US/docs/Web/API/Event

- .onclick
- .addEventListener
  - click
  - mouseover
- .preventDefault()

## Examples

- [jessica hische](http://jessicahische.is/)
- [color scheme switcher](https://github.com/ga-dc/color-scheme-switcher)

## You do: Events (5 min)
TODO: ???

## Conclusion (5 min)

1. What is the difference between a method and an attribute?
2. What is the difference between `onclick` and `addEventListener?`

## Break (10 min)
---

## Homework

<https://github.com/ga-dc/fellowship>
