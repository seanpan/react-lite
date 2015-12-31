# react-lite

## Introduction
React under 20k.
react-lite is an implementation of React that optimizes for small script size.

It supports the core APIs of React, such as Virtual DOM, intended as a drop-in
replacement for React, when you don't need server-side rendering in browser(no React.renderToString/React.renderToStaticMarkup).

If you are using webpack, it's so easy to use react-lite, just config alias in webpack.config.js:

```javascript
// webpack.config.js
{
	alias: {
		react: 'react-lite'
	}
}
```
## install

you can install react-lite from npm

```shell
npm install --save react-lite
```

## what can react-lite do?

just the same as what react do, see some demos below(I just make add alias from webpack.config.js, did'nt do anything else):

- react-lite work with react-router: [expamles](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/react-router-examples/index.html)
- react-lite work with redux:
	* [async](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/async/index.html)
	* [counter](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/counter/index.html)
	* [real-world](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/real-world/index.html)
	* [shopping-cart](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/shopping-cart/index.html)
	* [todomvc](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/todomvc/index.html)
	* [todos-with-undo](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/redux-examples/todos-with-undo/index.html)
- react-lite work with react-motion: [demos](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/react-motion-demos/index.html)
- js-repaint-perf(which is faster?):
	* [react](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/js-repaint-perf/react/index.html)
	* [react-lite](https://cdn.rawgit.com/Lucifier129/react-lite/master/examples/js-repaint-perf/react/lite.html)

## test
react-lite reuse react's unitest(155), you can see them in `__test__`, an run the test with:

```shell
npm test
```

License: MIT (See LICENSE file for details)