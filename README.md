# parse-sel

A "parse selector" kind of utility function.

## Install

With [npm](http://npmjs.com) do:

```bash
npm install parse-sel --save
```

## Usage

This module exports a function that takes a string with a [`hyperscript` selector](https://github.com/dominictarr/hyperscript) and returns an object.

```js
const parseSelector = require('parse-sel')

parseSelector('div#foo.bar')
// =>
// {
//   tagName: 'div',
//   id: 'foo',
//   className: 'bar'
// }
  
```

You can pass `true` as a second argument and get the `tagName` uppercase.

## Credits

This is mainly lifted from the [virtual-dom](https://github.com/Matt-Esch/virtual-dom) module.
[https://github.com/Matt-Esch/virtual-dom/blob/master/virtual-hyperscript/parse-tag.js](https://github.com/Matt-Esch/virtual-dom/blob/master/virtual-hyperscript/parse-tag.js)

There's also quite a few packages like this on [npm](http://npmjs.com).

## License

MIT
