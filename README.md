gazetteer
---

[![build status](https://secure.travis-ci.org/mapbox/gazetteer.png)](http://travis-ci.org/mapbox/gazetteer)

An index of places for styling maps, organized into a collection of machine-readable files.

### Usage

This package exports two functions:

* `get` for retrieving gazetteers by name.
* `lint` for checking if a JSON object conforms to [the gazetteer spec](./spec.md).

```js
import gazetteer from '@mapbox/gazetteer';

gazetteer.get('natural-label') // Returns a geoJSON FeatureCollection
gazetteer.lint(myGazetteerJson) // Returns an array of error messages
```

### Releasing

1. Run `npm version {major|minor|patch}`
1. Add an entry to the [`CHANGELOG`](./CHANGELOG.md) outlining the changes.
1. Create a pull request with the changes above.
