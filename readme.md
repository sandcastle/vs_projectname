# VS Project Name

[![Build Status](https://travis-ci.org/sandcastle/vs_projectname.svg)](https://travis-ci.org/sandcastle/vs_projectname)

A helper package for sanitizing Visual Studio project names with full
support for uni code character checking.

```js
var projectName = require('vs_projectname');

projectName('1badStart'); // _badStart
projectName('some name'); // some_name
projectName('noΩmath');   // no_math
```