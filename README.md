# country-flag-colors

Hex values of country flags. Based on https://vexillology.fandom.com/wiki/User:HansLN/National_flag_colors.

## Install

`npm install country-flag-colors`

## Usage

```js
var countryFlagColors = require("country-flag-colors");

console.log(countryFlagColors.find(f => f.name === 'Ireland').colors);

// ["#169b62", "#ffffff", "#ff883e"]
```

## Motivation

I was not able to find a list of countries and the colors of their flags in a JSON/CSV format, so I scraped the HTML from [HansLN National Flag Colors](https://vexillology.fandom.com/wiki/User:HansLN/National_flag_colors) and converted it to JSON.

I would also like to keep this package as light as possible, avoiding any external dependencies or transpilation, and the ability to use it as a one-line resource in your HTML. However,
I can envision adding helper methods like fetching all flags that contain specific hex values, grouping by continent/region, etc.

## Contributing

I am hoping to expand the functionality of this by narrowing down the primary colors of all flags. For example, El Salvador contains many individual
colors, but is primarily blue and white. There are also some colors that may be incorrect due to discrepancies in the source data.

Local flags could be added.

## License

MIT License

Copyright (c) 2024 Michael Joyce

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
