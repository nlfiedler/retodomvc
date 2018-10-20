# ReasonML TodoMVC Example

> Reason lets you write simple, fast and quality type safe code while leveraging
> both the JavaScript & OCaml ecosystems.

This project is a [todomvc](https://todomvc.com) example written in
[ReasonML](https://reasonml.github.io), using
[ReasonReact](https://reasonml.github.io/reason-react/en/) for rendering, and
[reductive](https://github.com/reasonml-community/reductive) for state
management.

## Learning ReasonML

The [ReasonML documentation](https://reasonml.github.io/docs/en/installation) is
the perfect guide to getting started with ReasonML.

* [Documentation](https://reasonml.github.io/docs/en/what-and-why)
* [API Reference](https://reasonml.github.io/api/index)
* [ReasonML on GitHub](https://github.com/facebook/reason)

### Videos

* [Ken Wheeler - ReasonML is Serious Business](https://www.youtube.com/watch?v=lzEweA7RPi0)
* [ReasonML by Jared Forsyth](https://www.youtube.com/watch?v=In4QEXThMxk)
* [ReasonConf videos](https://www.youtube.com/channel/UCtFP_Hn5nIbZY4Xi47qfHhw)

If you have other helpful links, or find any stale links above, please file an issue.

## Run Project

```sh
npm install
npm start
# in another tab
npm run webpack
```

After you see the webpack compilation succeed (the `npm run webpack` step), open
up `src/index.html` (**no server needed!**). Then modify whichever `.re` file in
`src` and refresh the page to see the changes.

## Build for Production

```sh
npm run build
npm run webpack:production
```

This will replace the development artifact `build/Index.js` for an optimized version.

**To enable dead code elimination**, change `bsconfig.json`'s `package-specs`
`module` from `"commonjs"` to `"es6"`. Then re-run the above 2 commands. This
will allow Webpack to remove unused code.
