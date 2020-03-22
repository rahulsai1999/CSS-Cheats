# Box Model and CSS Deep Dive

This section is dedicated to the box model.

### Hierarchy of Box Model

- `margin`
  - `border`
    - `padding`
      - `content`

---

### Margin Collapsing

- When two block elements are near each other, the bigger margin wins.
- This means margins are not repeated unless you use `margin-top` or `margin-bottom` specifically.

---

### Shorthand Properties

- combine the values of multiple properties in a single property
- **Examples**
  - `border : border-width border-style border-color`
  - `margin : top right bottom left`
  - `margin : top&bottom left&right`
  - `margin : all`

---

### Height, Width and Box Sizing Properties

- `section` and `div` are block level elements (HTML Features) which means they take up the **full available width by default**.
- Always pay attention to the relative height and width **or** absolute height and width.
- Height and Width are always applied with respect to the content i.e. `box-sizing : content-box` by default
- To make it include the padding and border, change it to `box-sizing : border-box`
