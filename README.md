WhatTheHechsher
===============
## Description
A hechsher is a symbol denoting the kosher status of a food item. It is a rabbinical certification noting that the food product is considered kosher in keeping with halakha (Jewish law), in accordance with the interpretation and stringencies held by that rabbinical organization.

Today, there are a lot of different hechsherim (plural of hechsher) from a number of different organizations. Some lists (such as the [Chicago Rabbinical Council, or CRC](http://www.crcweb.org/agency_list.php)) exist to point Jews to known "good hechshers", which follow acceptable practices according to their internal set of rules.

On this GitHub project, we intend to list all known hechshers, their symbols, and some supporting information. We intend for this to help future efforts for data projects. The data is located in the [data/data.json](data/data.json) file.

## Installation Instructions for Development
- Requires [node.js](https://nodejs.org/en/download/)
- Run `npm install` to grab the dependencies
- On commit and push, [husky](https://github.com/typicode/husky) will run [ajv-cli](https://github.com/jessedc/ajv-cli) to verify that data.json validates against schema.json

## Example
For example, the most widely-known hechsher is the OU, or Orthodox Union. Their symbol is: <img src="/images/OU.svg" width="20px" height="20px" />. Their entry in the data.json filewould look like this:

```
{
  "Organization Name": "Orthodox Union",
  "Short Name": "OU",
  "Symbol": "OU.svg",
  "Rabbi": "Rabbi Menachem Ganeck",
  "Website": "https://oukosher.org/"
}
```

The JSON data must match the schema.json file within the project, which contains restrictions and descriptions of each field.

## Disclaimer
The material collected here was gathered from existing online sources. We did not duplicate or utilize any existing copyrighted list or magazine.