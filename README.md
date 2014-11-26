# lint-deps [![NPM version](https://badge.fury.io/js/lint-deps.png)](http://badge.fury.io/js/lint-deps)

> CLI tool that tells you when dependencies are missing from package.json and offers you a choice to install them. Also tells you when dependencies are listed in package.json but are not being used anywhere in your project. Node.js command line tool and API.

## Install
## Install globally with [npm](npmjs.org):

```bash
npm i -g lint-deps
```

## API

```js
var deps = require('lint-deps');

// pass the directory to scan
console.log(deps('lib'));
```

## CLI

In the command line:

```bash
deps
```

### Commands

 - `-r` | `--report`: save a report to disk. By default `report.json` is saved. To change the path do: `-r foo.json`
 - `-e` | `--exclude`: comma-separated list of files or directories to exclude. Example: `deps -e test,lib`


## Examples

If packages are missing, you'll see a prompt like this:

![image](https://cloud.githubusercontent.com/assets/383994/2775405/1fb1c12a-cac5-11e3-8192-f379f412ad0a.png)

**If you choose <kbd>yes</kbd>:**

![image](https://cloud.githubusercontent.com/assets/383994/2775413/30b42c56-cac5-11e3-8ace-0999f0a75f48.png)

**choose dependencies**

![image](https://cloud.githubusercontent.com/assets/383994/2775421/43a349be-cac5-11e3-9cc6-20e9a3ae7f26.png)

**choose devDependencies**

![image](https://cloud.githubusercontent.com/assets/383994/2775427/518e5c76-cac5-11e3-8428-56a81dbd3f80.png)

**choose "nothing, just install"**

![image](https://cloud.githubusercontent.com/assets/383994/2775427/518e5c76-cac5-11e3-8428-56a81dbd3f80.png)

Now hit <kbd>enter</kbd> and everything that was checked will be installed.

**If you choose <kbd>no</kbd>:**

![image](https://cloud.githubusercontent.com/assets/383994/2775436/713003ea-cac5-11e3-9c69-eb3209531ccf.png)

Done.

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert  
Released under the MIT license

***

_This file was generated by [verb](https://github.com/assemble/verb) on November 21, 2014._