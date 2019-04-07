A typical **front end project setup**.


## Install & Run

In the repository root directory:

```sh
npm install
npm run dev
```

## Choices

Intended is to take the **most standard tooling** at the time of writing.

- `Webpack`: Is the "*runtime*": It 1) serves the files on `http://localhost:8080`, but also 2) orchestrates the pipeline to transform source files to servable files.
- `npm` as 1) the CL interface and 2) to manage frontend packages (at *development time*): It downloads libraries and keeps track of their versions and dependencies (in `package.json` and `package-lock.json`).
- `Babel` is a package that contains the logic to convert from ES5+ to browser-compatible ES5.

More precisely, the dependencies in `package.json`:

- `webpack` to bundle all the modules
- `webpack-cli` to run webpack from cli
- `webpack-dev-server` to serve the compiled file.
- `css-loader` to configure webpack for compiling the css
- `style-loader` loads all the css in the head of HTML
- `babel-loader` to configure webpack for using babel
- `@babel/core` to transpile the jsx to js
- `@babel/preset-env` to configure the transpiler for old browser

## Resources & Thanks

- [Amazing "what and why" of front end development tooling](https://medium.com/the-node-js-collection/modern-javascript-explained-for-dinosaurs-f695e9747b70).
- [Tutorial about how to bootstrap a React project](https://blog.bitsrc.io/setting-a-react-project-from-scratch-using-babel-and-webpack-5f26a525535d)
- [SASS for React?](https://www.quora.com/Should-I-use-Sass-for-React)

## Keywords
- **front end** (implies that `JavaScript` is executed **by the browser** aka client-side, **as opposed to server-side**).
- **setup** sums up that it is an actual project repository, but containing only the non-specific code.
- Possibly also related: _boilerplate_, _development environment_, _project bootstraping_.
