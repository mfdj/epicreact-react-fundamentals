**Context**

Working through [epicreact.dev/fundamentals](https://epicreact.dev/fundamentals)

Repository cloned/forked from [github.com/kentcdodds/react-fundamentals](https://github.com/kentcdodds/react-fundamentals)

**Project setup**

 - Forked at 2021 February 2: [7ba6f71](https://github.com/mfdj/epicreact-react-fundamentals/commit/7ba6f71f1ffee7ba819f4fa20f0bb19b8bbde81c)
 - Basic setup [#1](https://github.com/mfdj/epicreact-react-fundamentals/pulls/3) adds some personal prefrence config
 - Updating this README and run tests in CI [#3](https://github.com/mfdj/epicreact-react-fundamentals/pulls/3)
 - Drop docker + various docs [#4](https://github.com/mfdj/epicreact-react-fundamentals/pulls/4)
 - Drop matrix, just use ubuntu + node 14 [#5](https://github.com/mfdj/epicreact-react-fundamentals/pulls/5)
 
**Exercises**
 
1. Welcome [#1](https://github.com/mfdj/epicreact-react-fundamentals/pulls/3) adds some personal prefrence config
  * `npm run setup` [1c636ff](https://github.com/mfdj/epicreact-react-fundamentals/commit/1c636ff7bbe3a113d00cf98e4d404a191b52f759)
  * `npm test` works
1. Basic JS "Hello World" [#2](https://github.com/mfdj/epicreact-react-fundamentals/pulls/2)
  * my solution was pure js, whereas the final version used the root element directly in the html
  * learned that there is a [**module**](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/script#attr-type) type for script tags `<script type="module">…</script>` which does neat stuff like scope isolation for inline scripts (see: `extracurricular/script-type-node.html`)
