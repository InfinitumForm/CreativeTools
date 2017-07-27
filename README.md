# CreativeTools v1.x
Creative Tools is helper tools for all your works inside jQuery or Zepto

Creative Tools is made for faster and easyest orientation in javascript. Idea of Creativ Tools is to be more known-based approach to scripting. If you look in the code functions, you will see that some function names are similar to PHP functions and also work on the same way like `$.empty()`, `$.isset()`, `$.isNull()`, `$.date("m-d-Y")` , `$.time()`, `$.rot13(string)`, `$.base64_encode(string)`, `$.base64_decode(string)`, etc. which makes it easier to remember and use. Also Creative Tools support and have helpers for <a href="http://getbootstrap.com/" target="_blank">Twitter Bootstrap</a> and <a href="http://www.tinymce.com/" target="_blank">TinyMCE Editor</a>.

### Some cool Creative Tools features:

**Full Screen Responsive Box**
```
<div class="content-box">1</div>
<div class="content-box">2</div>
<div class="content-box">3</div>
<div class="content-box">4</div>

<script>
$(function($){
	$(function(){
		$(".content-box").fullScreen();
	});
});
</script>
```

**Save, edit, delete to HTML5 Local Storage**
```
if($.storage())
{
	// Set a session storage
	$.storage('the_storage', 'the_value');
	
	// Get session storage
	$.storage('the_storage');
	
	// delete storage
	$.storage('the_storage', null);
}
else
{
	// browser not support, use cookie
   	alert("WARNING!!! Your Browser is old and not have Web Storage support.\r\nPerhaps you'll have problems using this site.");
}
```

**Save, edit, delete Cookies**
```
// Set a session cookie
$.cookie('the_cookie', 'the_value');
$.cookie('the_cookie'); // -> 'the_value'

// Set a cookie that expires in 7 days
$.cookie('the_cookie', 'the_value', { expires: 7 });

// delete the cookie
$.cookie('the_cookie', null);
```

**Typing Preview**
```
<input name="text" type="text" id="text">
<div id="display"></div>
<div id="count-letters"></div>
<div id="count-words"></div>

<script>
$(function($){
	$("#text").typingPreview({
		text : '#display',
		count : '#count-letters',
		count_words : '#count-words'
	});
});
</script>
```

### Other cool stuffs you can find like
- Responsive
- Keyboard functions
- Content & Elements manipulation and checking functions
- Date & Time functions
- Transform operators
- Validators
- Page operators
- Bootstrap and WebKit popup
- and more...

This Creative Tools will grow up time to time. Please Fork this work and help me to develop this plugin to become better and useful.

Thanks!
