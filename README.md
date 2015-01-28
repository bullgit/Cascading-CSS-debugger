# Cascading-CSS-debugger
A cascading css debugger
----
A light-weight CSS debugger with super-powers ! 

To use it : 
- Download the style [cascading.css](https://raw.githubusercontent.com/bullgit/Cascading-CSS-debugger/master/cascading.css)
- Add the `debug` attribute to any element of your page ( `<div debug>...</div>` )
- Watch the cascading CSS debugger in action

----
To force the cascading debugger, or to have the whole DOM debugged, paste this line to your DevTool console :

javascript: 
```javascript
var allElements = document.querySelectorAll('*');

Array.prototype.forEach.call(allElements, function (element) {
  element.setAttribute('debug', '');
})

```
Or jQuery :
```javascript 
$(function(){
  var all = $('*');
  all.each(function(){
    $(this).attr('debug','');
  })
})
```

###Demo : 
<p data-height="268" data-theme-id="294" data-slug-hash="XJgOEV" data-default-tab="result" data-user="LukyVj" class='codepen'>See the Pen <a href='http://codepen.io/LukyVj/pen/XJgOEV/'>Cascading CSS debugger</a> by LukyVJ (<a href='http://codepen.io/LukyVj'>@LukyVj</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

2015 - bullg.it
