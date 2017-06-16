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

Blocks

.layout
  .layout__item
      .layout__item--fullwidth
      .layout__item--ninetycentered

.nav-primary

.header
  .header--primary

.sub-heading

.button
  .button--secondary
  .button--large

Notes:
- rename .layout-item as .layout-row and layout-item--* as layout-column-*?
- layout items have to have a max-width for super big screens