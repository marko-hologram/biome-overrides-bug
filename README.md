# Biome formatting overrides bug

Demonstrate how Biome `overrides` config option doesn't apply all formatter options that are specified, but only applies some. Haven't tested extensively what options are applied and what aren't.

## How to reproduce

1. run `npm install`
2. run `npm run format`
3. observe how in `main.js` object got force expanded and double quotes around console log first argument were added
4. observe how in `overrides/test.js` object was force expanded even though config specifies not to expand, but single quotes were added around console log argument as per overrides config