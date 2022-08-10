## Gazetteer

An index of places for maps, organized into a collection of machine-readable files that conforms to a [Gazetteer 1.1 spec](./gazetteer-spec/1.1/README.md).

### Usage

This package includes:

- A collection of Gazetteers
- A validation utility for verifying a JSON object conforms to the [Gazetteer 1.1 specification](./gazetteer-spec/1.1/README.md).

```js
import { worldwide, validate } from '@maplibre/gazetteer';

const { roadNetwork, settlements } = worldwide;

validate(roadNetwork); // Returns an array of error messages if invalid
```

### Releasing

1. Run `npm version {major|minor|patch}`
1. Add an entry to the [`CHANGELOG`](./CHANGELOG.md) outlining the changes.
1. Create a pull request with the changes above.
