# Tuts Plus: Bootstrap 3.0 Essentials

Learning Bootstrap with Tuts Plus

## Lesson 2-3 Grid System

### Classes

Column class naming is `col-<size>-<num columns to span>`. For example `col-lg-6`.
Size related notation refers to how that content will be displayed in the specified viewport.

There are 4 possible view port sizes that have corresponding notations, as described in the table below.

| Viewport             | Notation  | Notes                              |
|:-:                   |:-:        |:-:                                 |
|  Extra small devices | -xs       | Phones, < 768px                    |
|  Small devices       | -sm       | Tablets, >=768px                   |
|  Medium devices      | -mx       | Desktop, >= 992px                  |
|   Large devices      | -lg       | Large Desktop, >=1200px            |

Setting multiple col classes on a div sets up rules per viewport, for example:

  ```html
  <div class="col-lg-6 col-sm-4 col-xs-8">
    lorem ipsum dolor site amet...
  </div>
  ```

On extra small devices, this content would span 8 columns, on small devices 4 columns, and on large devices, 6 columns.

### Columns

Columns can be offset to the right by adding a specific class, for example `col-lg-offset-1`.

Columns can be nested provided they add up to 12.

Columns can be ordered differently using `pull` and `push` modifier classes.
`push` class moves column to the right, and `pull` class moves column to the left.