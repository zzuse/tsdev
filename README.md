# TSDev
## Project Package Generate -- package.json
`npm init -y`
## Installing (and updating) TypeScript 
`npm install -D typescript`  
Note: Not using `npm i -g typescript` Installing (and updating) TypeScript globally might break projects you haven’t touched in a while.

## Browser Utility
[Webpack](https://webpack.js.org)  
[ESBuild](https://esbuild.github.io) 

## Module Loading
```
The default converts module loading to CommonJS  
Setting module to `esnext` will use ECMAScript module loading
Two Module System
“// Entry-point for `import "dependency"` in ES Modules
"import": "./esm/index.js",
// Entry-point for `require("dependency") in CommonJS
"require": "./commonjs/index.cjs",”
```
----------

# TypeScript Project Init
`npx tsc --init` will generate tsconfig.json

# Include
```
"include": ["**/*.ts"],
```

## Run
`npx tsc`

## Describe
.d.ts, and as opposed to regular .ts files, its purpose is to hold declarations, no actual code.”

## Installing React
`npm install --save react`
### Installing React Type Definitions
`npm install --save-dev @types/react`

## Install Expressd JS Library for Backend Development
`npm install --save express`
### Install Express Type Definitions
`npm install -D @types/express @types/node` in current development env support node
### depend modules
npm install -D @types/lodash  
npm install -D preact

## Server/Client Side Run, need two tsconfig.json
`npx tsc -p server/tsconfig.json`  
`npx tsc -p client/tsconfig.json`

----------

# Test Framework
`npm install --save-dev mocha @types/mocha @types/node`

### In Memory TypeScript compilation
`npm install --save-dev ts-node`  
`npx mocha -r ts-node/register tests/*.ts`

### For Development Build Run
`npx tsc -p tsconfig.build.json`


### Remove Next Line Type Checking
// @ts-ignore
import _ from "https://esm.sh/lodash@4.17.21”

# Deno
https://docs.deno.com New Runtime, already include react  
configured by `deno.json`