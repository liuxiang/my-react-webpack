# 完整项目
```
cnpm install
```

# 使用yeoman generator
https://github.com/react-webpack-generators/generator-react-webpack#readme

## The following commands are available in your project:
```
  "scripts": {
    "start": "node server.js --env=dev",
    "test": "karma start",
    "test:watch": "karma start --autoWatch=true --singleRun=false",
    "posttest": "npm run lint",
    "serve": "node server.js --env=dev",
    "serve:dist": "node server.js --env=dist",
    "dist": "npm run copy & webpack --env=dist",
    "lint": "eslint ./src",
    "copy": "copyfiles -f ./src/index.html ./src/favicon.ico ./dist",
    "clean": "rimraf dist/*",
    "release:major": "npm version major && npm publish && git push --follow-tags",
    "release:minor": "npm version minor && npm publish && git push --follow-tags",
    "release:patch": "npm version patch && npm publish && git push --follow-tags"
  }
```
```
# Start for development
npm start # or
npm run serve

# Start the dev-server with the dist version
npm run serve:dist

# Just build the dist version and copy static files
npm run dist

# Run unit tests
npm test

# Auto-run unit tests on file changes
npm run test:watch

# Lint all files in src (also automatically done AFTER tests are run)
npm run lint

# Clean up the dist directory
npm run clean

# Just copy the static assets
npm run copy
```
