# Cascading-CSS-debugger
A cascading css debugger
----
A light-weight CSS debugger with super-powers ! 

To use it : 
- Download the style cascading.css
- Add the `debug` attribute to any element of your page
- Watch the cascading CSS debugger in action

----
To force the cascading debugger, or to have the whole DOM debugged, paste this line to your DevTool console :

```
$(function(){
  var all = $('*');
  all.each(function(){
    $(this).attr('debug','');
  })
})
```

2015 - bullg.it
