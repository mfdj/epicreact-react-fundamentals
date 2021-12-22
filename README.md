**Context**

Working through [epicreact.dev/fundamentals](https://epicreact.dev/fundamentals)

Repository cloned/forked from [github.com/kentcdodds/react-fundamentals](https://github.com/kentcdodds/react-fundamentals)

**Project setup**

 - Forked at 2021 February 2: [7ba6f71](https://github.com/mfdj/epicreact-react-fundamentals/commit/7ba6f71f1ffee7ba819f4fa20f0bb19b8bbde81c)
 - Basic setup [#1](https://github.com/mfdj/epicreact-react-fundamentals/pull/1) adds some personal prefrence config
 - Updating this README and run tests in CI [#3](https://github.com/mfdj/epicreact-react-fundamentals/pull/3)
 - Drop docker + various docs [#4](https://github.com/mfdj/epicreact-react-fundamentals/pull/4)
 - Drop matrix, just use ubuntu + node 14 [#5](https://github.com/mfdj/epicreact-react-fundamentals/pull/5)
 
**Exercises**
 
0. Welcome [#1](https://github.com/mfdj/epicreact-react-fundamentals/pull/1) adds some personal prefrence config
    * `npm run setup` [1c636ff](https://github.com/mfdj/epicreact-react-fundamentals/commit/1c636ff7bbe3a113d00cf98e4d404a191b52f759)
    * `npm test` works
0. Basic JS "Hello World" [#6](https://github.com/mfdj/epicreact-react-fundamentals/pull/6)
    * my solution was pure js, whereas the final version used the root element directly in the html
    * learned that there is a [**module**](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script#attr-type) type for script tags `<script type="module">…</script>` which does neat stuff like scope isolation for inline scripts (see: `extracurricular/script-type-node.html`)
0. Intro to Raw Reacts APIs [#6](https://github.com/mfdj/epicreact-react-fundamentals/pull/6)
    * converting our "Hello World" to React; uses [`React.createElement`](https://reactjs.org/docs/react-api.html#createelement) and [`ReactDOM.render`](https://reactjs.org/docs/react-dom.html#render)
    * "Because React exposes a UMD, which is short for Universal Module Definition, it allows us to create a global variable in the browser that we can reference inside of our code" 💡 this is a good reminder that UMD is useful for non-code-bundler situations
    * great article [Imperative vs Declarative Programming](https://ui.dev/imperative-vs-declarative-programming/)
    * `React.createElement` just returns objects
    * DOM manipulation is namespaced `ReactDOM` because compilation target is abstracted away (i.e. also React Native and React VR)
0. Using JSX [#7](https://github.com/mfdj/epicreact-react-fundamentals/pull/7)
    * Definitely want to make not of the [Babel REPL](https://babeljs.io/repl#?browsers=defaults%2C%20not%20ie%2011%2C%20not%20ie_mob%2011&build=&builtIns=App&corejs=3.6&spec=false&loose=false&code_lz=MYewdgzgLgBArgSxgXhgHgCYIG4D40QAOAhmLgBICmANtSGgPRGm7rNkDqIATtRo-3wMseAFBA&debug=false&forceAllTransforms=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=react&prettier=true&targets=&version=7.16.6&externalPlugins=&assumptions=%7B%7D)
    * GTK that `@babel/standalone@7.12.4/babel.js` + `<script type="text/babel">` are available!
    * the [extra credit video](https://epicreact.dev/modules/react-fundamentals/using-jsx-extra-credit-solution-01) has a great breakdown of why `<Thing propA={…}>{…}</Thing>` allows expressions inside the js-interpolated `{…}` and not statements (because it compiles down to `React.createElement(Thing, { propA: … }, …)`)
    * also good https://reactjs.org/docs/jsx-in-depth.html
