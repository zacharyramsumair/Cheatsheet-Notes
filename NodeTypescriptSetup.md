tsc --init

make some changes to the tsconfig
•  "target": "es2016",  to
    "target": "es6", 

• "rootDir": "./", to
"rootDir": "./src",

• "outDir": "./", to
"outDir": "./build",

make build and src folders


uncomment 
"moduleResolution": "node" -> and set it just to node instead of node10


 "scripts": {
    "start": "node ./build/app.js",
    "build": "tsc -p .",
    "dev": "nodemon ./src/app.ts"
  },
