A simple repo to help reproduce why the fern CLI is not passing through the deprecated status of openapi schema properties.

You can reproduce the issue by running:

```
npm install
npm run docs:definition
```

The property `otherFertiliserType` in `CottonCrop.json` has the flag `deprecated: true` but the entry in `__package__.yml` has no corresponding attribe of `availability: deprecated`
