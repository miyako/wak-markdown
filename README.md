wak-markdown
============

Wakanda module to convert MD to HTML using the libmarkdown library.

About
-----
* [Discount](http://www.pell.portland.or.us/~orc/Code/markdown/)/2.1.6

![obsolete-word-black-frame-word-obsolete-word-black-frame-d-rendering-123942590](https://user-images.githubusercontent.com/1725068/78463940-29122280-771e-11ea-8be8-a7830725403e.jpg)

Old Wakanda.

Example
-------
```js
var modulesFolder = FileSystemSync('Modules');
var markdown = require(modulesFolder.path + 'markdown');

var html5 = false;//use html5 tags;default=0
var github = false;//github flavour markdown;default=0
var html = '* 1 abc';

markdown.convert(html, html5, github).toString();//returns Blob, as it may or may not be utf-8
//<ul><li>1 abc</li></ul>
```
**Note**: The input html can be string or Buffer.
