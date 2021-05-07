# DIY Grid Based Framework

## About
* Framework made as a means to learn Sass.

<br>

## Grid
The grid module allows you to create a container with rows or columns to create layouts.

### Columns
* Designate the container with `.columns`.
* Direct children of the container automatically become columns.
* Columns will take up an equal amount of space by default.

#### Sizing and positioning columns
* Change the percentage width of a column with a class in the form of `.is-`*`n`*, where *n* is a number from 1 to 100.
* If the total width of your columns does not reach 100%, you can choose how to distribute your columns in the remaining space. Place one of the following classes on your container:

    | Class  | Effect |
    | ------------- | ------------- |
    | .has-columns-centered  | Columns will be centered in the container.  |
    | .has-columns-left  | Columns will be far left in the container.  |
    | .has-columns-right  | Columns will be far right in the container.  |
    | .has-columns-spaced-between  | Remaining free space will be placed between columns.  |
    | .has-columns-spaced-around  | Remaining free space will be placed around columns.  |
    | .has-columns-spaced-evenly  | Remaining free space will be placed between and around columns.  |

### Rows
* Designate the container with `.rows`.
* Direct children of the container automatically become rows.
* Rows will be as tall as their contents.

### Gutters
* You can place 10px gutters between your rows or columns by placing `.has-gutters` on the container.

<br>

## Positioning
The positioning module enables various tools for adjusting the spacing and positioning of elements.

### Containers
Assigning the `.container` class to an element will center it and it's contents horizontally. By default a container will of a medium(m) size. You can change this by choosing between 5 container sizes by using a class of the form `.container-`*`size`*, where *size* is either **xs, s, m, l** or **xl**.

| Class  | Container Width |
| ------------- | ------------- |
| .container-xs  | 50%  |
| .container-s  | 60%  |
| .container  | 70%  |
| .container-m  | 70%  |
| .container-l  | 80%  |
| .container-xl  | 90%  |

<br>

### Padding and Margin
You can place padding and/or margin on any element by assigning a class to it in the form of *`.td-s`*, where *t* is one of the following values:

| *t* | Type |
| ------------- | ------------- |
| p | Padding  |
| m | Margin |

<br>

and *d* is one of the following values:

| *d* | Direction |
| ------------- | ------------- |
| t | Top  |
| r | Right |
| b | Bottom |
| l | Left |
| x | Left and Right |
| y | Top and Bottom |

<br>

and *s* is one of the following values:

| *s* | Size |
| ------------- | ------------- |
| 1 | 0.25rem  |
| 2 | 0.5rem |
| 3 | 0.75rem |
| 4 | 1rem |
| 5 | 1.25rem |
| 6 | 1.5rem |

<br>

### Position Properties
You can apply a position property to an element with one of the following classes:

| Class | Result |
| ------------- | ------------- |
| .is-static | position: static |
| .is-relative | position: relative |
| .is-absolute | position: absolute |
| .is-fixed | position: fixed |

<br>

### Offset Properties
You can assign offset properties to an element to change it's position relative to it's parent. (Remember that you need to assign `.is-relative`, `.is-absolute` or `.is-fixed` to both the parent element and the child element you are trying to position.)

| Class | Result |
| ------------- | ------------- |
| .is-top-left | top: 0; left: 0; |
| .is-top-middle | top: 0; left: 50%; right: 50%; |
| .is-top-right | top: 0; right: 0; |
| .is-bottom-left | bottom: 0; left: 0; |
| .is-bottom-middle | bottom: 0; left: 50%; right: 50%; |
| .is-bottom-right | bottom: 0; right: 0; |
| .is-center-left | top: 50%; left: 0%; transform: translate(0%, -50%); |
| .is-center-middle | top: 50%; left: 50%; transform: translate(-50%, -50%); |
| .is-center-right | top: 50%; left: 100%; transform: translate(-100%, -50%); |