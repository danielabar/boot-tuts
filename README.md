# Tuts Plus: Bootstrap 3.0 Essentials

Learning Bootstrap with Tuts Plus

## Lesson 2.3 Grid System

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

## Lesson 2.4 Glyphicons Icon Font

Icons rendered as font rather than image (old bootstrap 2) for optimized display on all screen sizes and resolutions.

Icons can be used on their own, for example to display a star:

  ```html
  <span class="glyphicon glyphicon-star"></span>
  ```

Icons can also be used with other components such as buttons:

  ```html
  <button type="button" class="btn btn-primary">
    <span class="glyphicon glyphicon-user"></span>
  </button>
  ```

Note that icons will change color depending on the control they're residing in.

## Lesson 2.5 List Group

List groups are super-charged list items.

Can also add badges, will get pushed to the right.

Can also add heading to each list item.

## Lesson 2.6 Panel

Simple bordered box containing some content.

Can have header, footer, and contain list groups and tables.

Can also have context (primary, info, etc.)

## Lesson 2.7 Navbar and Modals

Navbar starts collapsed in mobile view, and becomes horizontal as viewport gets wider.

Use classes `navbar-right` and `navbar-left` to align elements at left or right of navbar respectively
(used to be `pull-right` and `pull-left` in bootstrap 2).

Modal is responsive and does not have a max height. As more content is added to it, it will expand to fill the view port.

## Lesson 2.8 Removed Components

Accordian: Can achieve similar effect using collapse.js plugin, together with panel component.

Typeahead: Instead use [twitter typeahead](https://github.com/twitter/typeahead.js/)

## Lesson 2.9 Customizer

Bootstrap can be [customized](http://getbootstrap.com/customize/)

Many LESS variables are exposed for customization.

Media query breakpoint and layout/grid system can also be customized.

Also try [bootstrap-generator-less](https://github.com/Thomas-Lebeau/generator-bootstrap-less) for yeoman scaffolded project setup with LESS compile process to fully customize bootstrap.

## Lesson 2.10 Browser Support

Good for all modern browsers.  Few issues on older IE.

IE8 doesn't support border-radius, box-shadow, transform, transition, and placeholder.

IE9 won't support transition and placeholder.

Furthermore, IE8 doesn't support media queries, use a polyfill like [Respond.js](https://github.com/scottjehl/Respond)

Ensure latest rendering mode is used for IE support by adding following meta tag:

  ```html
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  ```