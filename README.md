# node with typescript and postgresql

## typescript installed as a local package
`npm install typescript --save-dev`
in package.json
"scripts": {
    ...
    "tsc": "tsc"
}
`npm run tsc -- --init`

tsconfig.json file will be generated and replace it with following:
{
 "compilerOptions": {
 "module": "commonjs",
 "esModuleInterop": true,
 "target": "es6",
 "moduleResolution": "node",
 "sourceMap": true,
 "outDir": "dist/src"
},
 "lib": ["es2015"]
}