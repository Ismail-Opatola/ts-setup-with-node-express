# Typscript Setup with Nodejs + Express

<!-- Run watch mode in terminal
    `tsc types.ts -w` -->

install typscript 

`npm i -g typscript`

To create tsconfig file 

run `tsc --init` 

open the config file and uncomment needed settings

* point the `rootDir` and `outDir`

    - `"rootDir": "./src"` --- specify our ts files
    - `"outDir": "./dist"` --- specify path to dump compiled js output
    - `"watch": true` --- watch changes
    - `"target": "es6"` --- compile to es6
    - `"moduleResolution": "node"` --- use node

run `tsc` in terminal


