# Underscore Template Auto-Escape

[Underscore.js](http://documentcloud.github.com/underscore/) is great.

However, its default template function doesn't auto-escape interpolations. Fooey!

See:

* <https://github.com/documentcloud/underscore/issues/129>
* <https://github.com/dvv/underscore/commit/a4f4d30440f52c7cef26e8574e8eae384a66db9f>

## Installation

Include `underscore-template-autoescape.js` (or the minified version) after `underscore.js`.

## Usage

`_.template(…)` will now automatically escape values when using the
``<%= … %>` interpolation. If you wish to use the traditional, non-escaped
interpolation, use `<%- … %>`.

Bonus: `_.escapeHTML(string)` will HTML escape strings.
