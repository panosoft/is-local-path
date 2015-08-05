# is-local-path

Test whether a path is local.

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
