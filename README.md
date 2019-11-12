# vue loader plugin

## Explaination
this is a rewrite of VueLoaderPlugin to solve the compatibility with webpack5

webpack5 has rewrited the ruleset module, which means the VueLoaderPlugin cannot use class `Ruleset` any more, instead, it should using the `RuleSetCompiler`


## Installation
```bash
npm i --save-dev vue-loader-plugin
yarn add --dev vue-loader-plugin
```

## usage

- before
    ```js
    // webpack.config.js
    const VueLoaderPlugin = require('vue-loader/lib/plugin')

    module.exports = {
        // ...
        plugins: [
            new VueLoaderPlugin()
        ]
    }
    ```


- now
    ```js
    // webpack.config.js
    const VueLoaderPlugin = require('vue-loader-plugin');
    module.exports = {
        // ...
        plugins: [
            new VueLoaderPlugin()
        ]
    }
    ```