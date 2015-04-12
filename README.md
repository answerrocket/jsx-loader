# React JSX loader for webpack

## Usage:

```js
{..., loader: 'jsx-loader?harmony&es6module'}
```

You must install [`react-tools`](https://www.npmjs.com/package/react-tools) as a
peer dependency, ideally pegged to the same version of React that you use at runtime.

To enable ES6 features, use `?harmony` and/or `?es6module` in your loader config.

[Flow]-style type annotations can be stripped using `?stripTypes`.

In general, any flag that `react-tools`'s `transform` `options` parameter will
accept may be provided as a query parameter to this loader.

This fork has been updated to apply source maps from previous loaders to the source map output by
`react-tools`.

[Flow]: http://flowtype.org/
