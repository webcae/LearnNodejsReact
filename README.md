## Learn Node.js
### Node.js -> DOCS -> Guides
- [x] Getting Started Guide (https://nodejs.org/en/docs/guides/getting-started-guide/)
- [ ] https://nodejs.dev/learn (Node.js -> learn)
- Quick start
  - Open-Source, Cross-platform, V8 engine, single thread, asynchronous I/O, only javaScript, new ECMAScript standards use npm to manage vast number of libs
  - Base flow:
    - require('http') -> http.createServer -> server.listen
  - Some platforms:
    - Express, Loopback.io, Meteor, Micro, Nx, Socket.io
  - History: 2009 - 
  - How much JavaScript do you need?
  - use Babel to transform your code to be ES5-compatible (browser javascript) 
- Getting Start
  - JS engine (V8 and others)
  - Interpretation and Compilation(just-in-time (JIT))
  - Run Node.js scripts -> $> node app.js
  - Exit from a Node.js program -> Ctrl+C, process.exit(), SIGTERM, process.kill(process.pid, 'SIGTERM')
  - Access environment variables -> process.env.XXX
  - REPL -> CommandLine interactive mode, tab key -> auto complete, Dot commands(.help)
  - Accept arguments from the command line -> process.argv.forEach(), process.agrv.slice(), require('minimist')(process.argv.slice(2))
  - Output to the command line
    - console.log(), %s, %d, %i, %o, console.clear(), console.count(), console.trace()
    - time(), timeEnd()
    - stdout, stderr
    - color the output, Chalk lib (npm install chalk)
    - progress bar in console, progress lib (npm install progress)
  - Accept input from the command line -> readline module, but readline-sync package is more simple, and Inquirer.js package
  - How to use exports -> module.exports, 1) module.exports = somefunc 2) exports.somefunc = somefunc 3) exports.somefunc = {}
  - npm -> "npm install" from "package.json", --save / --save-dev option, "npm update"
  - Runing task -> npm run <task-name>, task is script defined in package.json, also Webpack
  - Location of npm install -> npm install -g <package-name> for global installation
  - How to use or execute a package
    - library    -> require('lib_name') 
    - executable -> npx exe_fileName (which is installed under node_module/.bin folder)
  - package.json -> name, author, contributors, bugs, homepage, version, license, keywords, description, repository, main, private, scripts, dependencies, devDependencies, engines, browserslist, Command-specific properties, Package vesions
  - package-lock.json -> It sets your currently installed version of each package in stone, and npm will use those exact versions when running npm install. The dependencies versions will be updated in the package-lock.json file when you run npm update.
  - How to find the installed version of an npm package -> npm list, npm list -g, npm list --depth=0, npm list packageName, npm list dependencyPackName, npm view packageName version
  - How to Install an older version of an npm package -> npm install package@version
  - How to update all the Node.js dependencies -> npm outdated, npm install -g npm-check-updates -> ncu -u -> npm update or npm install.
  - Semantic Versioning using npm -> all versions have 3 digits: major.minor.patch
  - Uninstalling npm packages -> npm uninstall [-S -D -g] package-name
  - npm global or local packages -> In general, all packages should be installed locally. A package should be installed globally when it provides an executable command that you run from the shell (CLI), and it's reused across projects. [npm list -g --depth 0]
  - npm dependencies and devDependencies -> The package is automatically listed in the package.json file [-S, -D], npm install --production
  - The npx Node.js Package Runner -> npx lets you run code built with Node.js and published through the npm registry. [npx commandname], [npx node@10 -v], [npx https://gist.github.com/zkat/4....]
  -   
  - The Node.js Event Loop
  
  
  
  
   
### Learn Express

### Learn React
