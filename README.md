# typescript-empty-project

Simplistic TypeScript empty project:

- Install [node.js](https://nodejs.org/):
  - on Ubuntu: `sudo apt-get install nodejs-legacy`
  - on Mac with Homebrew: `brew update && brew install node`
- To start developing, just type:

  ```bash
  # Install dependencies locally
  npm i
  # Starts a server with live-reload, and recompiles files when they're saved:
  npm start
  ```
  
- To build a self-contained deployable artefact (`build/index.html`):

  ```
  npm run build
  ```

About this setup:

- TypeScript with strict settings (null-awareness, no implicit any, no implicit returns) and down-compilation to ES5
- Optimized bundle creation with Rollup + Uglify
- Immutable.js import to get you started with decent collections :-)
- Inlines all .js into `build/index.html` when running `npm run build`

What it does not do:

- No Angular2 setup. It's not ready yet for `--strictNullChecks` and has its own command line tool anyway.
- No React / Flux setup. Should be easy to use, though.
