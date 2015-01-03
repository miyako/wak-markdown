wak-markdown
============

Wakanda module to convert MD to HTML using the libmarkdown library.

About
-----
* [Discount](http://www.pell.portland.or.us/~orc/Code/markdown/)/2.1.6

Example
-------
```js
var modulesFolder = FileSystemSync('Modules');
var markdown = require(modulesFolder.path + 'markdown');

var html5 = false, github = false;
var html = '* 1 abc';

markdown.convert(html5, github, html);//<ul><li>1 abc</li></ul>
```
**Note**: The input/output can be string or Buffer.
