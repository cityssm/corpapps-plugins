# Third Party Plugin Inventory

The City's internal corporate applications platform relies on several third-party plugins *to get the job done*!
Since the applications are internal, the browser support requirements are less sticky,
and are limited to the browsers on City-issued devices.

## Main Plugins

**[RequireJS](http://requirejs.org/)**
- Loads the JavaScript files required to make each application page work (and nothing more).

**[jQuery 3](http://jquery.com/)**
- A Bootstrap prerequisite.
- Originally used for more, but moving away from in favour of native browser feature support.

**[Bootstrap 3](https://getbootstrap.com/)**
- The component library that keeps us from having to spend time writing components.

**[Font Awesome 4](https://fontawesome.com/)**
- The icon library for the applications.

## Polyfill Plugins

*Mainly to stay current while preserving Internet Explorer 11 support, but also older Android phones.*

- [Array.prototype.find](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/find#Polyfill)
- [Element.prototype.closest](https://developer.mozilla.org/en-US/docs/Web/API/Element/closest#Polyfill)
- [window.fetch](https://github.com/github/fetch)
- [window.Promise](https://github.com/taylorhakes/promise-polyfill)
- [window.URLSearchParams](https://github.com/WebReflection/url-search-params)

## Other Plugins (Alphabetical Order)

| Plugin | Purpose |
| ------ | ------- |
| [Autosize](https://github.com/jackmoore/autosize) | Adjusts textarea height automatically to accommodate text. |
| [Bootstrap Datepicker](https://github.com/uxsolutions/bootstrap-datepicker) | |
| [jQuery Sparklines](https://omnipotent.net/jquery.sparkline/) | Renders small graphs inside some application search results. |
| [Leaflet](https://github.com/Leaflet/Leaflet) | Plots application records on a map. |
| [Marked](https://github.com/markedjs/marked) | Converts Markdown to HTML using JavaScript. |
| [Random Color](https://github.com/davidmerfield/randomColor) | Generates good looking random colors. |
