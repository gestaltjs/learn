# Learn
📚 A structured learning journey to get familiar with the Javascript, Node, and Web ecosystems.

## How to use it

Continue reading through this `README.md` file. The content in this file will guide you through resources, questions, and exercises to consolidate the different areas of knowledge.

## Themes

### 1. Javascript

Javascript is the language that powers GestaltJS and the apps that developers build with it. It's a language that emerged to make the web dynamic, and that popularized to the point that it can be used in any imaginable platform: [*Anything that can be Written in JavaScript, will Eventually be Written in JavaScript*](https://www.typemock.com/anything-that-can-be-written-in-javascript-will-eventually-be-written-in-javascript/). We don't need to know everything about Javascript to build software with it. However, we need to be familiar with the most basic units of composition and the syntax to write software that's readable, well-architected and testable. If you need to learn further about any Javascript concept or API, you can use the wonderful [mdn web docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript) from Mozilla.

#### Read

- [Functions](https://www.w3schools.com/js/js_functions.asp)
- [Rest parameters](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters)
- [Javascript classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
- [What are Pure Functions and Side Effects in JavaScript?](https://blog.greenroots.info/what-are-pure-functions-and-side-effects-in-javascript)
- [How to use promises](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Promises)
- [I/O-bound vs CPU-bound in Node.js](https://bytearcher.com/articles/io-vs-cpu-bound/)
- [Javascript engines](https://en.wikipedia.org/wiki/JavaScript_engine)

#### Questions
- When would you use plain Javascript objects and when classes?
- What are the risks of building stateful software?
- When would you use promises and when async/await?
- If runtimes execute code in a single thread, how is asynchrony achieved?
- Is Javascript more suitable for CPU or IO bound software?
- What's the difference between a Javascript runtime and a engine?

#### Exercises

- Create a website that through Javascript, it fetches the latest tweets from the [@gestaltjs](https://twitter.com/gestaltjs) account and presents them in the page through [DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction) manipulation.
- Use [Javascript modules](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules) to split up the above script into smaller reusable modules.

### 2. Tooling

One aspect that characterizes Javascript is the need for additional tooling to work with it: [Babel](https://babeljs.io/), [Webpack](https://webpack.js.org/), [Rollup](https://rollupjs.org/guide/en/), [Vite](https://vitejs.dev/)... For someone learning Javascript fo the first time, it might look surprising that one can't just write Javascript and execute it in the browser or the NodeJS runtime. Many people developing Javascript these days do so without having a good understanding on why the tooling is necessary. However, understanding the role those pieces play, will be beneficial long term. For example, you'll be able to debug issues yourself, or optimize your workflows as the project scales. In this section we'll dive into a bit of history to understand why the tooling is necessary, how they've evolved over time, and how a future without tooling might be possible soon.

#### Read

- [What is Babel?](https://babeljs.io/docs/en/)
- [WTF is a Source Map](https://www.schneems.com/2017/11/14/wtf-is-a-source-map/)
- [Faster than webpack: JavaScript bundling with esbuild](https://blog.logrocket.com/fast-javascript-bundling-with-esbuild/)
- [Why Vite](https://vitejs.dev/guide/why.html)
- [Webpack and Rollup: the same but different](https://medium.com/webpack/webpack-and-rollup-the-same-but-different-a41ad427058c)
- [Polyfill](https://developer.mozilla.org/en-US/docs/Glossary/Polyfill)

#### Questions
- What is a Polyfill?
- What are the pros and cons of Babel?
- How does ESBuild compare to Webpack?
- How does Rollup compare to Webpack?
- What does Vite offer that Webpack doesn't?
- What are the limitation of Javascript processors written in compiled languages?
- What'll be necessary to eliminate the need for additional tooling?
- Why are sourcemaps necessary?
#### Exercises

- Write a Node application in Typescript and use [`@babel/node`](https://babeljs.io/docs/en/babel-node) with the [`@babel/preset-typescript`](https://babeljs.io/docs/en/babel-preset-typescript) to run your application.
- Use [esbuild](https://github.com/evanw/esbuild) to bundle and output your application into `dist/`. Output sourcemaps.
- Add a script that uses [esmo](https://github.com/antfu/esbuild-node-loader) to run your application directly.
- Repeat the esbuild step but use [Rollup](https://rollupjs.org/guide/en/) to output the bundle into `dist/`. Output sourcemaps.
- Repeat the esbuild step but use [swc](https://swc.rs/).
- Create a [Vite](https://vitejs.dev/) application with an `index.html` and a client-side Vue application that mounts in the DOM.
#### Resources
- [caniuse](https://caniuse.com/): "Can I use" provides up-to-date browser support tables for support of front-end web technologies on desktop and mobile web browsers.


## 3. Module system