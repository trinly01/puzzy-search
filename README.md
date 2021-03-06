[![npm version](https://badge.fury.io/js/puzzy-search.svg)](https://badge.fury.io/js/puzzy-search)

# puzzy-search
Add google-like `search` and `auto suggest` (did you mean...)

 - [x] misspelled words
 - [x] fuzzy search
 - [x] suggest similar words

<p align="center">
  <img src="search.gif"/>
</p>

> **Join and support our Community** <br />
> Web and Mobile Developers PH <br />
> [ [Facebook Page](https://fb.com/webmobile.ph) | [Group](https://fb.com/groups/webmobile.ph/) ]

## Install
```
npm install puzzy-search
```

## CDN
```html
  <script src="https://unpkg.com/puzzy-search/dist/index.js"></script>
```

## Usage
```js
const { search, suggest, regex } = require('puzzy-search')
// const { search, suggest, regex } = puzzySearch // for CDN

const sentence = 'You want the web server to support four of the most popular programming paradigms.'

const str = 'puppular programmng paradim'

search(str, sentence) // true

suggest(str, sentence) // popular programming paradigm

regex(str) // new RegExp(...puzzy...)

sentence.match(regex(str)) !== null // true
```


# *Join and support our Community* <br /> **Web and Mobile Developers PH** <br/> [ [Facebook Page](https://fb.com/webmobile.ph) | [Group](https://fb.com/groups/webmobile.ph/) ]

## License
ISC © 2019 Trinmar Boado
MIT © 2019 Ray Foss
MIT © 2017 Arve Seljebu
