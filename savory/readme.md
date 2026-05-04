<!-- readme.md -->

- X grid-template-areas 
- X justify-items 
- X justify-content 
- X justify-self
- X align-items
- X align-content
- align-self
- grid-auto-rows
- grid-auto-columns
- grid-auto-flow

# Justify Items

- There are two axes in a grid layout - the *`column`* (or block) axis and the *`row`* (or inline) axis.

- The *column* axis stretchs from top to bottom across the web page.

Justify Items
8 min
We have referred to “two-dimensional grid-based layout” several times throughout this course.

There are two axes in a grid layout — the column (or block) axis and the row (or inline) axis.

The column axis stretches from top to bottom across the web page.

The row axis stretches from left to right across the web page.

In the following four exercises, we will learn and use properties that rely on an understanding of grid axes.

justify-items is a property that positions grid items along the inline, or row, axis. This means that it positions items from left to right across the web page. This property is declared on grid containers.

justify-items accepts these values:

start — aligns grid items to the left side of the grid area
end — aligns grid items to the right side of the grid area
center — aligns grid items to the center of the grid area
stretch — stretches all items to fill the grid area
There are several other values that justify-items accepts, which you can read about on the Mozilla Developer Network. The definitions for these values can also be found in the documentation. It is important to note that the page with the definitions includes some values that are not accepted in CSS Grid layout.

<main>
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</main>

Copy to Clipboard

main {
  display: grid;
  grid-template-columns: repeat(3, 400px);
  justify-items: center;
}

Copy to Clipboard

In the example above, we use justify-items to adjust the positioning of some elements on this web page.

There is a grid container with three columns that are each 400 pixels wide.
The container has three grid items that do not have a specified width.
Without setting the justify-items property, these elements will span the width of the column they are in (400 pixels).
By setting the justify-items property to center, the .card <div>s will be centered inside of their columns. They will only be as wide as necessary to contain their content (the words Card 1, etc).
If we specify a width for the .card elements, they will not stretch the width of their column.
Instructions
Checkpoint 1 Enabled
1.
Look in style.css. Each column inside of the <main> element is 250 pixels. The recipes stretch to take up the entire 250 pixels.

In the .recipe ruleset, add the width property and set its value to 200px.

What changes?

Checkpoint 2 Step instruction is unavailable until previous steps are completed
2.
In the main ruleset, add a justify-items property with the value center.

The elements won’t be completely centered just yet. Depending on your browser size, you may not notice much of a move at all. We’ll learn why in the following exercise!

- `justify-items` position elements within their columns.


