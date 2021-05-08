# DIY Grid Based Framework

## About
Framework made as a means to learn Sass. Split into modules so the framework can be as light as necessary.

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

<br>

## Typography
The typography module includes various classes for styling and aligning text.

<br>

### Font Family
The [Lato Typeface](https://fonts.google.com/specimen/Lato) is used for all elements if available, or a compatible sans serif font will be used if not.

<br>

### Titles
Each title class will set the text to be bold and a certain size. Title classes come in the form `is-title-`*`n`*, where *n* is a number from 1 to 6:

| Class | Result |
| ------------- | ------------- |
| .is-title-1 | font-size: 20px; font-weight: bold; |
| .is-title-2 | font-size: 30px; font-weight: bold; |
| .is-title-3 | font-size: 40px; font-weight: bold; |
| .is-title-4 | font-size: 50px; font-weight: bold; |
| .is-title-5 | font-size: 60px; font-weight: bold; |
| .is-title-6 | font-size: 70px; font-weight: bold; |

<br>

### Text Alignment
You can align text to either the left, center or right with the classes `.has-text-left`, `.has-text-center` and `.has-text-right`. Placing one of these classes of a container will align all text within it accordingly. Place a class on a single element to align its text individually.

<br>

### Font Weight
To choose a font weight use a class of the form `.has-text-`*`weight`*, where *weight* is either **thinner**, **thin**, **regular** or **bold**:

| Class | Font Weight |
| ------------- | ------------- |
| .has-text-thinner | 100 |
| .has-text-thin | 300 |
| .has-text-regular | 400 |
| .has-text-bold | 700 |

<br>

### Font Size
To choose a font size use a class of the form `.is-fs-`*`size`*, where *size* is a number from 1 to 6:

| Class | Font Size |
| ------------- | ------------- |
| .is-fs-1 | 12px |
| .is-fs-2 | 15px |
| .is-fs-3 | 18px |
| .is-fs-4 | 25px |
| .is-fs-5 | 30px |
| .is-fs-6 | 35px |

<br>

### Colors
You can use the **lighter**, **light**, **neutral**, **dark** or **darker** suffixes to use greyscale text. More colorful options include **danger**, **warning**, **success** and **primary**.

| Class | Color |
| ------------- | ------------- |
| .has-text-lighter | #c9c9c9 |
| .has-text-light | #adadad |
| .has-text-neutral | #838383 |
| .has-text-dark | #474747 |
| .has-text-darker | #252525 |
| .has-text-danger | #f14d4d |
| .has-text-warning | #f6f861 |
| .has-text-success | #5cf370 |
| .has-text-primary | #4c7de6 |

<br>

### Italics and Underlines
You can make text italic with `.has-text-italic`, and/or underline it with `.has-text-underlined`.