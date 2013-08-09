# NOTE: obsolete

You're free to use this library, but since it was written, Underscore has started including autoescaping in its core, so this library is no longer necessary.

See http://underscorejs.org.  Usage:

* ``_.escape`` Escapes HTML
* ``<%- ... %>`` Escaped HTML in templates
* ``<%= ... %>`` Raw (unescaped) strings in templates.

In short: Just use ``<%- ... %>`` in place of ``<%= ... %>`` and you get escaped text with underscore.

If you want to confuse people and swap the default behaviors of these functions, continue reading. :)

----

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

# License

Copyright (c) John Nishinaga

Redistribution and use of this software in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
3. Neither the name of Yahoo! Inc. nor the names of YUI's contributors may be used to endorse or promote products derived from this software without specific prior written permission of Yahoo! Inc.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. 
