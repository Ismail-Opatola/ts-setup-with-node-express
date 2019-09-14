# Typscript Setup with Nodejs + Express
Using typscript on the Backend

<!-- Run watch mode in terminal
    `tsc types.ts -w` -->

install typscript 

`npm i -g typscript`

To create tsconfig file 

run `tsc --init` 

open the config file and uncomment needed settings

<!-- * point the `rootDir` and `outDir` -->

    "rootDir": "./src" --- specify our ts files
    "outDir": "./dist" --- specify path to dump compiled js output
    "watch": true --- watch changes
    "target": "es6" --- compile to es6
    "moduleResolution": "node" --- use node

run `tsc` in terminal

install express

`npm i express`

install dev dependencies

`npm i -D typescript ts-node nodemon @types/node @types/express`


Edit `Package.json` file

    "scripts": {
    "start": "node dist/app.js",
    "dev": "nodemon src/app.ts",
    "build": "tsc -p ." 
    },

development mode

`npm run dev`

once you're ready to build

run `npm run build`

it should create a `./dist` folder with compiled `app.js`

to run the server

run `npm start`

app.js is served, :ghost: yey!
