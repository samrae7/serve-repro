Demo of issue I am having with npm module serve: https://www.npmjs.com/package/serve

Issue opened here: https://github.com/zeit/serve/issues/477


## Setup
- `npm install`
- `serve -s`
- Note that if you go to eg. `localhost:5000/foo` the js files is loaded in the page but if you go to `localhost:5000/foo/bar` it can no longer found it and so tries to load the index.html as the bundle.js. Error you get in the console is:
`Uncaught SyntaxError: Unexpected token <`