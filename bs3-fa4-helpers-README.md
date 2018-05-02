# bs3-fa4-helpers.css

Some additional CSS used in the City's corporate application that ties together
Bootstrap 3 and Font Awesome 4.


## .form-control-noresize

Removes the resize option from a textarea.

```html
<textarea class="form-control form-control-noresize"></textarea>
```

## .form-control-nospinner

Removes the nuisance spinner (up and down arrow buttons) from a number input field.

**Sample Usage HTML**

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
