## text_color

The `textcolor` component adds the forecolor/back color button controls that enables selecting colors from a color picker and applying them to text. It adds a toolbar button and menu item to allow this functionality.

**Type:** `String`

##### Example

```js
tinymce.init({
  selector: "textarea",
  menu: {
    format: { title: "Format", items: "forecolor backcolor" }
  },
  toolbar: "forecolor backcolor"
});
```

### Options

These settings affect the execution of the `textcolor`. The dimensions and mapping of the grid of text colors can be set here.

### `color_cols`

This option allows specifying the number of columns that can appear on the grid of text colors. The number of rows is calculated based on how many text colors are supplied divided by the specified number of columns.  The `textcolor_cols` and `textcolor_rows` property has been removed in TinyMCE 5.0.

**Type:** `String`

**Default Value:** `"5"`

##### Example

```js
tinymce.init({
  selector: "textarea",  // change this value according to your HTML
  toolbar: "forecolor backcolor",
  color_cols: "5"
});
```
### `color_map`

This option allows specifying a map of the text colors that will appear in the grid.

**Type:** `Array`

##### Example

```js
tinymce.init({
  selector: "textarea",  // change this value according to your HTML
  toolbar: "forecolor backcolor",
  color_map: [
    "000000", "Black",
    "993300", "Burnt orange",
    "333300", "Dark olive",
    "003300", "Dark green",
    "003366", "Dark azure",
    "000080", "Navy Blue",
    "333399", "Indigo",
    "333333", "Very dark gray",
    "800000", "Maroon",
    "FF6600", "Orange",
    "808000", "Olive",
    "008000", "Green",
    "008080", "Teal",
    "0000FF", "Blue",
    "666699", "Grayish blue",
    "808080", "Gray",
    "FF0000", "Red",
    "FF9900", "Amber",
    "99CC00", "Yellow green",
    "339966", "Sea green",
    "33CCCC", "Turquoise",
    "3366FF", "Royal blue",
    "800080", "Purple",
    "999999", "Medium gray",
    "FF00FF", "Magenta",
    "FFCC00", "Gold",
    "FFFF00", "Yellow",
    "00FF00", "Lime",
    "00FFFF", "Aqua",
    "00CCFF", "Sky blue",
    "993366", "Red violet",
    "FFFFFF", "White",
    "FF99CC", "Pink",
    "FFCC99", "Peach",
    "FFFF99", "Light yellow",
    "CCFFCC", "Pale green",
    "CCFFFF", "Pale cyan",
    "99CCFF", "Light sky blue",
    "CC99FF", "Plum"
  ]
});
```
### `custom_colors`

This option allows disabling the custom color picker in all color swatches of the editor.

**Type:** `Boolean`

**Default Value:** `true`

##### Example

```js
tinymce.init({
  selector: "textarea",  // change this value according to your HTML
  toolbar: "forecolor backcolor",
  custom_colors: false
});
```
