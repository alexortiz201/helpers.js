# helpers.js

A collection of small JavaScript helper functions for various use cases. All of these little snippets solve problems that are very common, but don't have a widespread decent implementation. Most functions are available as easy-to-use prototypes on their respective objects.

---

## Number

### Number.round

Rounds a number to a given precision and omits trailing 0 values.

```js
100.51235.round(3)
```

    100.512

## String

### String.base

Gets only the base of a given URL.

```js
'https://www.twitter.com/RadLikeWhoa_'.base()
```

    'twitter.com'

### String.format

Format a string using placeholders like `{0}`.

```js
'{0}, hello {1} world!'.format('Oh', 'beautiful')
```

    'Oh, hello beautiful world!'

### String.insert

Insert a string into another one at a given numerical index or a keyword.

```js
'I am here.'.insert('in between ', 5)
```

    'I am in between here.'

### String.truncate

Truncates the string to the given length and replaces superfluous characters with the given substitute.

```js
'This is a longer text'.truncate(15)
```

    'This is a long…'

### String.words

Count the words inside a given element. The output can be formatted using the `{{count}}` placeholder.

```js
'Hello, world!'.words()
```

    2

## Functions

### readingtime

Returns the estimated time to complete reading of a text in a human readable format.

```js
readingtime(2720, 'Reading this takes {time}.', 270)
```

    'Reading this takes about 10 minutes.'