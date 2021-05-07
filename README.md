# DIY Grid Based Framework

## About
* Framework made as a means to learn Sass.

## Docs

### Columns
* Designate the container with `.columns`.
* Direct children of the container automatically become columns.
* Columns will take up an equal amount of space by default.

    #### Sizing and positioning columns
    * Change the percentage width of a column with a class in the form of `.is-`*`n`*, where *n* is a number from 1 to 100.
    * If the total width of your columns does not reach 100%, you can choose how to distribute your columns in the remaining space. Place one of the following classes on your container:
        * `.has-columns-centered`: Columns will be centered in the container.
        * `.has-columns-left`: Columns will be far left in the container.
        * `.has-columns-right`: Columns will be far right in the container.
        * `.has-columns-spaced-between`: Remaining free space will be placed between columns.
        * `.has-columns-spaced-around`: Remaining free space will be placed around columns.
        * `.has-columns-spaced-evenly`: Remaining free space will be placed between and around columns.

### Rows
* Designate the container with `.rows`.
* Direct children of the container automatically become rows.
* Rows will be as tall as their contents.

### Gutters
* You can place 10px gutters between your rows or columns by placing `.has-gutters` on the container.