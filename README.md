# retodomvc

A [todomvc](https://todomvc.com) example written in
[ReasonML](https://reasonml.github.io), using
[ReasonReact](https://reasonml.github.io/reason-react/en/) for rendering, and
[reductive](https://github.com/reasonml-community/reductive) for state
management.

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
