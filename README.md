## Opinionated JavaScript Snippets for Sublime Text 3

A more opinionated for version of https://github.com/jprichardson/sublime-js-snippets, following current best practices.  Designed with strict linters in mind.

<!-- MarkdownTOC -->

- [Install](#install)
  - [via package control](#via-package-control)
  - [directly on Mac OS X](#directly-on-mac-os-x)
- [The Snippets](#the-snippets)
  - [Vanilla Snippets](#vanilla-snippets)
    - [](#afn)
    - [](#bea)
    - [](#bei)
    - [](#bes)
    - [](#cd)
    - [](#ce)
    - [](#cl)
    - [](#cli)
    - [](#ct)
    - [](#fn)
    - [](#ii)
    - [](#iius)
    - [](#me)
    - [](#okfe)
    - [](#pe)
    - [](#proto)
    - [](#req)
    - [](#sto)
    - [](#sti)
    - [](#us)
  - [BDD Snippets (Behavior-Driven Development)](#bdd-snippets-behavior-driven-development)
    - [](#desc)
    - [](#ita)
    - [](#its)
- [Inspiration](#inspiration)
- [More on Sublime Text Packages](#more-on-sublime-text-packages)

<!-- /MarkdownTOC -->


## Install

### via package control
Install via package control: http://wbond.net/sublime_packages/community Search for **JavaScript Snippets** or typically the keywords **js** or **javascript** are suitable.

### directly on Mac OS X

```sh
git clone git:/github.com/levbrie/js-snippets.git /Users/YOUR_USER_NAME/Library/Application\ Support/Sublime\ Text\ 3/Packages/
```

## The Snippets

### Vanilla Snippets

#### [afn] anonymous function

```javascript
function (${1:arguments}) {
  ${0:// body...}
}
```

#### [bea] beforeEach async

```javascript
beforeEach(function () {
  ${1:// body...}
});
```

#### [bei] beforeEach angular inject

```javascript
beforeEach(inject(function(${1:depsToInject}) {
  ${2://make injected deps available}
}));
```

#### [bes] beforeEach synchronous

```javascript
beforeEach(function () {
  ${1:// body...}
});
```


#### [cd] console.dir

```javascript
console.dir(${1:obj})${0}
```


#### [ce] console.error

```javascript
console.error(${1:error})${0}
```


#### [cl] console.log

```javascript
console.log(${1:msg})${0}
```


#### [cli] console.log with util.inspect

```javascript
console.log(require('util').inspect(${1:obj}, true, ${2:10}, true))${0}
```


#### [ct] console.trace

```javascript
console.trace(${1:msg})${0}
```


#### [fn] function

```javascript
function ${1:methodName}(${2:arguments}) {
  ${0:// body...}
}
```

#### [ii] Immediately-invoked function expression

```javascript
(function () {
  ${0:// body...}
})();
```

#### [iius] Immediately-invoked function expression with 'use strict'

```javascript
(function () {
  'use strict';
  ${0:// body...}
})();
```

#### [me] module.exports

```javascript
module.exports = ${1}
```


#### [okfe] Objects.keys and forEach

```js
Object.keys(${1:obj}).forEach(function(key) {
  ${0:// body...}
})
```


#### [pe] process.exit

```javascript
process.exit()
```


#### [proto] prototype

```javascript
${1:ClassName}.prototype.${2:methodName} = function(${3:arguments}) {
  ${0:// body...}
}
```


#### [req] require

```javascript
require('${1:package}')${0}
```


#### [sto] setTimeout

```javascript
setTimeout(function() {
  ${2:// body...}
}, ${1:millis})
```


#### [sti] setInterval

```javascript
setInterval(function() {
  ${2:// body...}
}, ${1:millis})
```


#### [us] use strict

```javascript
'use strict'
```



### BDD Snippets (Behavior-Driven Development)

#### [desc] describe

```javascript
describe('${1:description}', function() {
  ${0:// body...}
});
```


#### [ita] asychronous it

```javascript
it('${1:description}', function(done) {
  ${0:// body...}
});
```


#### [its] synchronous it

```javascript
it('${1:description}', function() {
  ${0:// body...}
});
```



## Inspiration

Originally forked from and almost entirely based on/inspired by [JP Richardson's sublime-js-snippets](https://github.com/jprichardson/sublime-js-snippets) - I just tend to follow stricter coding practices with semicolons and the like.

## More on Sublime Text Packages

For info on creating and submitting packages to package control go to:
https://packagecontrol.io/docs/submitting_a_package
