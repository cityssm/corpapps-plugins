# bs3-fa4-helpers.css

Some additional CSS used in the City's corporate application that ties together
Bootstrap 3 and Font Awesome 4.

Note that our application uses vanilla Bootstrap, so some theming may be required.


## .alert-absolute-bottom, .alert-fixed-bottom

Sticks an alert to the the bottom of the page or the browser window.

```html
<div class="alert alert-warning alert-fixed-bottom">
  You have unsaved changes.
</div>
```


## .form-control-highlight-invalid

Automatically highlights a form-control with invalid input using the `:invalid` CSS selector.
Similar to including ```.has-error``` on the parent ```.form-group```.

*May require some color changes to fit your theme.*

```html
<input class="form-control form-control-highlight-invalid" type="number" min="0" step="1" />
```


## .form-control-noresize

Removes the resize option from a textarea.

```html
<textarea class="form-control form-control-noresize"></textarea>
```

## .form-control-nospinner

Removes the nuisance spinner (up and down arrow buttons) from a number input field.

```html
<input class="form-control form-control-nospinner" type="number" />
```


## .fa-rotate-animate

Used alongside Bootstrap 3's collapse and dropdown plugins.
When the dropdown is expanded, the right caret rotates 90 degrees to point down.
Simply include the ```.fa-rotate-animate``` class on the icon inside the toggle button.

**Sample Dropdown Usage HTML**

```html
<div class="btn-group">
  <button class="btn btn-default dropdown-toggle" data-toggle="dropdown" type="button" aria-haspopup="true" aria-expanded="false">
    Reports <span class="fa fa-caret-right fa-rotate-animate"></span></button>
  <ul class="dropdown-menu dropdown-menu-right">
    <li>
      <a href="#">
        <span class="fa fa-download"></span> Download Report 1
      </a>
    </li>
  </ul>
</div>
```

**Sample Collapse Usage HTML**

```html
<div class="panel panel-default">
  <div class="panel-heading">
    <h2 class="panel-title">
      <a class="btn-block" data-toggle="collapse" href="#searchFilters" role="button">
        Search Filters
        <span class="fa fa-fw fa-rotate-animate fa-caret-right pull-right"></span>
      </a>
    </h2>
  </div>
  <div class="panel-collapse collapse" id="searchFilters" role="tabpanel">
    <div class="panel-body">
      <div class="form-group">
        <label for="filter--searchStr">Search String</label>
        <input class="form-control" id="filter--searchString" name="searchString" type="text" />
      </div>
    </div>
  </div>
</div>
```

## .label-fa

Replaces the standard HTML input checkbox or radio button with a Font Awesome icon.

*Styling automatically applies to `label.list-group-item`.*

**Sample HTML**

```html
<label class="label-fa">
  <input type="checkbox" />
  <span class="fa fa-fw fa-lg fa-square-o radio-fa"></span>
  Remember Me
</label>
```

## .panel > .tab-content > .list-group

Adjust margins and borders for ```.list-group``` elements used as ```.tab-pane``` s inside of ```.panel``` s.
Modelled after styles applied to ```.list-group``` divs that appear inside ```.panel-collapse``` divs.

**Sample HTML**

```html
<div class="panel panel-default">
  <div class="panel-heading">
    <h2 class="panel-title">Panel Title</h2>
  </div>
  <div class="panel-body">
    <ul class="nav nav-pills" role="tablist">
      <li class="active" role="presentation">
        <a data-toggle="tab" href="#tab-1" role="tab" aria-controls="tab-1">Tab 1</a>
      </li>
      <li role="presentation">
        <a data-toggle="tab" href="#tab-2" role="tab" aria-controls="tab-2">Tab 2</a>
      </li>
    </ul>
  </div>
  <div class="tab-content">
    <div class="tab-pane list-group active" id="tab-1" role="tabpanel">
      <div class="list-group-item"></div>
      <div class="list-group-item"></div>
      <div class="list-group-item"></div>
    </div>
    <div class="tab-pane list-group" id="tab-2" role="tabpanel">
      <div class="list-group-item"></div>
      <div class="list-group-item"></div>
      <div class="list-group-item"></div>
    </div>
  </div>
</div>
</div>
```
