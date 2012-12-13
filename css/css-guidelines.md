CSS Guidelines
==============

A guide to writing CSS code

## Code Style

* Use soft-tabs with a two space indent.
* Put spaces after : in property declarations.
* Put spaces before { in rule declarations.
* Use hex color codes #000 unless using rgba.
* Hex codes to be uppercase.
* Class names are lowercase with hypens
* Class names have meaningful names

```css
.time-widget {
	border: 1px solid #CECECE;
	color: #F00;
	background: rgba(0,0,0,0.6);
}
```

### Naming conventions

Use names that are specific and reflect the purpose of that element. Use generic names where needed.

**Keep Things Generic**

Keep class names as short as possible, but don't compromise readibility

```css
/* Generic */
.nav {}

/* Specific */
.time-widget-handle {}

/* Bad */
.navigation {}
.atr {}

/* Good */
.nav {}
.author {}
```

**No Tags**

Avoid using elements in selectors. There should be no need to use them and also helps with performance

```css
/* Bad */
ul.nav {}
span.error {}

/* Good */
.nav {}
.error {}
```

**Shortcodes**

Use shortcodes where possible.

```css
/* Bad */
.widget {
	padding-top: 10px;
	padding-right: 5px;
	padding-bottom: 10px;
	padding-left: 5px;
	border-top-color: #CCC;
	border-top-style: solid;
	border-top-width: 1px;
	color: #FF0000;
}

/* Good */
.widget {
	padding: 10px 5px;
	border: 1px solid #CCC;
	color: #F00;
}
```

**Namespacing**

Use namespacing to help maintain code and prevent conflicts with other code

```css
/* Good */
.time-widget {}
.time-widget-clock-face {}
.time-widget-big-handle {}
.time-widget-little-handle {}
```

**States**

When using a class to describe a state, make sure it falls within a namespace

```css
/* Bad */
.selected {}
.disabled {}

/* Good */
.time-widget-clock-face.selected {}
.time-widget-clock-face.disabled {}
```

### Formatting Rules

Use a semi-colon after every line. Add a space after every colon. Add a space before curly brace.

```css
/* Bad */
.widget{
	background: #F00;
	color:#FFF
}

/* Good */
.widget {
	background: #F00;
	color: #FFF;
}
```

Separate selectors onto a new line

```css
/* Bad */
a, a:hover, a:focus {
	color: #F00;
}

/* Good */
a,
a:hover,
a:focus {
	color: #F00;
}
```