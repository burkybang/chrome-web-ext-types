# chrome-web-ext-types

TypeScript type definitions for WebExtensions polyfill to be used with Chrome based on MDN's documentation.

## Requirements

As this library is using the `object` type and default values for generics,
`typescript` should at least be on version `2.3` to get the definitions to work.

## Install It

```sh
# yarn version
yarn add burkybang/chrome-web-ext-types --dev

# npm version
npm install --save-dev burkybang/chrome-web-ext-types
```

As this is not a [`DefinitelyTyped`][definitely-typed] package, you will have to
include the type definition in your `tsconfig.json` by hand, via a `typeRoots`
option.

```json5
{
  "compilerOptions": {
    // You have to explicitly set @types to get DefinitelyTyped type definitions
    "typeRoots": ["node_modules/@types", "node_modules/chrome-web-ext-types"],
  }
}
```

[definitely-typed]: https://github.com/DefinitelyTyped/DefinitelyTyped
