# Repro for create-react-app / yarn berry bug

This repo was created by:

1. create `package.json` with workspace setup
1. `mkdir packages`
1. `cd packages`
1. `yarn dlx create-react-app app --template typescript`
1. `rm -rf app/.git app/.yarn app/yarn.lock app/.pnp.js`
1. `yarn`
1. `cd app`
1. `yarn start`

The error message I get is:

```
Failed to compile.

TypeScript error in undefined(undefined,undefined):
Cannot find type definition file for 'jest'.  TS2688
```
