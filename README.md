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
