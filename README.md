# is-local-path

Test whether a path is local.

[![npm](https://img.shields.io/npm/v/is-local-path.svg)]()
[![Travis](https://img.shields.io/travis/panosoft/is-local-path.svg)]()
[![David](https://img.shields.io/david/panosoft/is-local-path.svg)]()
[![npm](https://img.shields.io/npm/dm/is-local-path.svg)]()

## Installation

In npm, do

	npm install is-local-path
	
## Usage

	var isLocalPath = require('is-local-path');
	
	isLocalPath('/path/to/file.ext')); // true
    isLocalPath('/path/to/directory')); // true
    isLocalPath('./relative/path')); // true
    isLocalPath('../relative/path')); // true
    isLocalPath('data:text/plain;base64,SGVsbG8sIFdvcmxkIQ%3D%3D')); // false
    isLocalPath('http://host.com/path/to/file.ext')); // false
