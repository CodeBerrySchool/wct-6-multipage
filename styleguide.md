# Style Guide

## Principles we use in this project

- It should be modular / component-based to promote reuse and easier maintenance in the future.
- It shouldn't be as complicated as a full BEM architecture, it should just introduce the student to object oriented CSS.

## Style principles

### 1. The Single Responsibility Principle

One piece of code (in this case a class) should do one thing and one thing only.

### 2. The Open/Closed Principle

Entities should be open for extension but closed for modification. 

### 3. The Separation of Concerns

## Architecture

- Block » standalone entity that is meaningful on its own.
- Element » a part of a block that has no meaing on its own and is semantically tied to its block.
- Modifier » a flag on a block or an element, use them to change appearance or behavior.

Should text be its own block? 
Nope, it's not BEM-like. The resetting is harder this way but it will be solved by using preprocessors.


Notes:
- rename .layout-item as .layout-row and layout-item--* as layout-column-*?
- layout items have to have a max-width for super big screens
- reindent everything and add meaningful whitespace upon refactor
- refactor the 3-column grid based on the four-column grid
- the map embed is broken so far.. a bigger aspect ratio might help. maybe equal to the video? also it needs an overlay toprevent scrolling.
- fix the company data » how to center it without losing text-align? nest in another layout item maybe? » nest it in a div and make the div inline-block » ul buttons can be hidden with padding 0
- div card: h3 h4 (csak előrébb), ul, li, button, span
- bodyra kerüljön a font-family
- link together pages in navs
- buttons need a hove and a click state
- the placeholder text is badly positioned. how to add padding-left?
- link in mailchimp somehow?
- is it okay to have a fixed width / height for buttons?