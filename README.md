> **Warning**
> This project is no longer maintained, it is replaced by the work of the DFINITY teams [see forum](https://forum.dfinity.org/search?q=svelte)

# dfx_svelte_poc

Recipe to setup Svelte with Internet Computer starting from  __dfx new__

## Create dfx project

`dfx new <my_project>`

## Install extra svelte

```
npm install --save svelte svelte-loader;
npm install --save-dev mini-css-extract-plugin;
npm install --save-dev css-loader;
```

## update webpack.config.js

see __diff_with_webpack_dfx_011.pdf__

## update source

* __./src/<my_project>_frontend/src/App.svelte__
* __./src/<my_project>_frontend/src/index.html__
* __./src/<my_project>_frontend/src/index.js__

## Try it!

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/rbolog/dfx_svelte_poc)
