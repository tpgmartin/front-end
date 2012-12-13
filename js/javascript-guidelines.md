JavaScript Guidelines
=====================

A guide to writing JavaScript code

## Semicolons

Use semicolons at the end of assignmenets. It will reduce the risk of issues of errors occuring.

```js
// bad
var getFilm = function() {
	return "The Legend of Ron Burgundy"
}

// good
var getFilm = function() {
	return "The Legend of Ron Burgundy";
}
```

## Variables

Always declare variables with `var`. This improves readibility and helps prevent clashes with variables in the global scopes (i.e. window scope).

```js
// bad
anchorman = 'Ron Burgundy';

// good
var anchorman = 'Ron Burgundy';
```

## Strings

Use single quotes when defining strings

```js
// bad
var anchorman = "Ron Burgundy";

// good
var anchorman = 'Ron Burgundy';
```


## Objects

When creating objects, use the literal syntax

```js
// bad
var obj = new Object();

// good
var obj = {};
```

Never use reserved words in JavaScript. (<a href="https://gist.github.com/4275925">see list here</a>)

```js
// bad
var anchorman = {
  class: 'you stay classy San Diego',
  default: {drink: 'Scotch'},
  with: 'Veronica Corningstone'
};

// good
var anchorman = {
  quote: 'you stay classy San Diego',
  defaults: {drink: 'Scotch'},
  partner: 'Veronica Corningstone'
};
```

To maximise readability, structure objects like so:

```js
// bad
var perfume = {name: 'Sex Panther',maker: 'Odeon',scent: 'pungent'}

// good
var perfume = {
  name: 'Sex Panther',
  maker: 'Odeon',
  scent: 'pungent'
}
```

## Arrays

When creating array, use the literal syntax

```js
// bad
var arr = new Array();

// good
var arr = [];
```

When pushing to an array, if the array length is known then use the direct assignment over Array#push. (<a href="http://jsperf.com/array-direct-assignment-vs-push/11">Performance Tests</a>)

```js
// bad
var bicepCurls = [],
    i;

// bad
for (i = 0; i < 100; i++) {
  bicepCurls.push(i * 10);
}

// good
for (i = 0; i < 100; i++) {
  bicepCurls[i] = i * 10;
}
```

If the length is unknown, then use Array#push

```js
var bicepCurls = [],

// bad
bicepCurls[bicepCurls.length] = 'two tickets to the guns show';

// good
bicepCurls.push('two tickets to the guns show');
```

If you need to copy an array, use the Array constructor (<a href="http://jsperf.com/converting-arguments-to-an-array/7">Performance Tests</a>)

```js
var len = oldStore.length,
    newStore = [],
    i;

// bad
for (i = 0; i < len; i++) {
  newStore[i] = oldStore[i];
}

// good
newStore = Array.apply(null, oldStore);
```

To maximise readability, structure arrays like so:

```js
// bad
var perfume = [];
prefume[0] = 'London Gentleman';
prefume[1] = 'Blackbeard's Delight';
prefume[2] = 'Sex Panther';

// good
var perfume = ['London Gentleman', 'Blackbeard's Delight', 'Sex Panther']
```

### Naming conventions