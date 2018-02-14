To reproduce the issue:

```
yarn
yarn test
```


The error currently received is:

```
 src/App.test.js
  ● Test suite failed to run

    ReferenceError: Component is not defined

      at _get_original__ (src/App.js:18:2203)
      at _get__ (src/App.js:18:1945)
      at Object.<anonymous> (src/App.js:5:19)
      at Object.<anonymous> (src/App.test.js:3:12)
          at <anonymous>
      at process._tickCallback (internal/process/next_tick.js:188:7)
```

This error goes away if the `babel` key in `package.json` is removed
