# Initial Steps for New Project (React/Parcel)

## A. Initial Project Setup

1. Create project folder
2. Create src directory in the project folder
3. Run `npm init -y` to create a package.json file
4. Run `git init` to initialize project as a git repository
5. Create a .gitignore file to add files that don't need to be pushed to github
6. Add node modules to git ignore file

## B. Build Process

Bundlers are used to bundle Javascript modules into a single Javascript files that can be executed in the browser. This setup is using Parcel

1. Install parcel - `npm i -D parcel-bundler`
2. Create an index.html file in the src directory
3. Create an index.js file in the src directory
4. Create a script in package.json to launch dev server
   - `"dev": "parcel src/index.html` (this gives parcel the entry point of index.html)
   - run `npm run dev` to run the application
5. Add all the output of parcel to git ignore
   - dist/
   - .cache/

## C. Code Style

### PRETTIER - more about how the code works

1. install formatting tool - Prettier - `npm install -D prettier`
2. add a file .prettierrc to the root of the project

   - add {} in the .prettierrc file or add other configurations

3. install prettier extension (if not installed already)
4. Go to settings
   - check command on save
   - check require config

### EDITORCONFIG - code formatting rules

1. create a new file .editorconfig in the root directory
2. check editor config doc for configuration
3. install editor config extension (if not already installed)

### ESLINT - more about the style, about what the code does

1. install eslint `npm install -D eslint eslint-plugin-import eslint-config-prettier`
2. create a new file in the root directory - .eslintrc.json
3. configure eslint by putting settings in the eslintrc file
4. install eslint ext (if not already installed)

## D. Testing

1. install jest - `npm install -D jest`
2. add to package.json - `"test": "jest"`

## E. REACT

1. install react and react-dom - `npm install react react-dom`
2. install babel - `npm i -D babel-preset-env babel-preset-react`
3. create a .babelrc file in root directory
   - include `{ "presets" : ["env", "react"] }`
4. create components folder in src directory
5. create styles folder in src directory
