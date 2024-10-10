# minimal-reproduction-template

First, read the [Renovate minimal reproduction instructions](https://github.com/renovatebot/renovate/blob/main/docs/development/minimal-reproductions.md).

## Current behavior

```bash
export LOG_LEVEL=debug
export RENOVATE_TOKEN=ghp_....
npx renovate --autodiscover=true --autodiscover-filter='splincode/renovate-reproductions'
```

Renovate nothing to update

## Expected behavior

I expect bumped minimal range version

```json5
{
  // ...
  "peerDependencies": {
    // ...
    "@maskito/angular": ">=3.1.0 <4",
    "@maskito/core": ">=3.1.0 <4",
    "@maskito/kit": ">=3.1.0 <4",
    "@maskito/phone": ">=3.1.0 <4",
    "@ng-web-apis/common": ">=4.9.0 <5",
    "@ng-web-apis/intersection-observer": ">=4.9.0 <5",
    "@ng-web-apis/mutation-observer": ">=4.9.0 <5",
    "@ng-web-apis/resize-observer": ">=4.9.0 <5"
  }
}
```

Explain the expected behavior here.

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/31883
