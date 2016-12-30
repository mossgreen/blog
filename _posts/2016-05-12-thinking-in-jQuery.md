---
layout: post
title: Thinking in jQuery
---

These are my notes while reading some blogs(e.g., http://www.ruanyifeng.com) and the book [jqfundamentals](http://www.jqfundamentals.com/).
The content will be the following:

### 1. How to select DOM elements

    the basic design concept of JQ is that it selects an element from DOM and manipulate it directly.

1.1 the select expression can be CSS selectors:

```
$(document) // to select whole document object
$('#myId') // to select the element whose ID is myId
$('div.myClass') // to select the element whose class is myclass
$('input[name=first]') // the input element whose name attribute is 'first'
```

1.2 the select expression can also be JQ expression:
	
```
$('a:first') // to select the first element in the page
$('tr:odd') // to select odd rows
$('#myform :input') // to select input element in the form
$('div:visible') // to select visible elements
$('div:gt(2)') //to select all div elements except the first three (index starts from 0)   
$('div:animated') // to select those elements that is currently animating
```

### 2. How to change the result sets
3. Chaining 
4. DOM manipulating: get and set values
5. DOM manipulating: movement
6. DOM manipulating: copy and create  elements
7. Tools
8. Event
9. Special effect
