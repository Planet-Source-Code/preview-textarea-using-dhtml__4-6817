<div align="center">

## Preview TextArea Using DHTML\.


</div>

### Description

This is a small script that will allow you to preview a textarea in an html page that may contain html code with out first processing the page to another page. May sound complicated but you will see it's not. This is for people who don't want to create a preview page just to re-write the textarea. It can now be done on the same page as the text area!.
 
### More Info
 
You send the ID tag of the textarea you want to popup.

This is a script that needs IE. It might even need IE 5.0, but I'm not sure.

No Returns

None that I can think of.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[N/A](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/empty.md)
**Level**          |Intermediate
**User Rating**    |4.0 (8 globes from 2 users)
**Compatibility**  |ASP \(Active Server Pages\), HTML, VbScript \(browser/client side\)

**Category**       |[ASP Server Object Model](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/asp-server-object-model__4-32.md)
**World**          |[ASP / VbScript](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/asp-vbscript.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/preview-textarea-using-dhtml__4-6817/archive/master.zip)

### API Declarations

No CopyRight, But please let me know if you use this or change it .. I love to see new ideas.


### Source Code

```
<html>
<SCRIPT LANGUAGE=jscript>
var oPopup = window.createPopup();
function DisplayHTML(handl){
oPopup.document.body.innerHTML = window.document.all(handl).innerText;
oPopup.document.body.style.border = "solid black 1px";
oPopup.show(10,20, 400, 200, event.srcElement);
}
</script>
<BODY>
The TextArea Below Support HTML Tags
<br><TEXTAREA rows=10 cols=30 name=txtNote ID=txtNote>
<ul>
<li>Item1</li>
<br>
<li>Item 2</li>
</ul>
</TEXTAREA><span id=ttxtNote style="cursor:hand; font-weight:bold" onmouseover="DisplayHTML('txtNote')" onmouseout="oPopup.hide()" >PreView</span>
</BODY>
</html>
```

