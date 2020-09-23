<div align="center">

## Text Box Jump


</div>

### Description

This script will allow you to jump from one text box to the next when a desired length is reached.
 
### More Info
 
ObjName --> Name of Text Box

ObjNum --> Max characters to be typed before jumping

to call this function place the following code in your text box instantiation --> onkeyup="NextBox('text_box_name',value to jump at(int));"


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Michael R Brown](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/michael-r-brown.md)
**Level**          |Beginner
**User Rating**    |4.8 (19 globes from 4 users)
**Compatibility**  |
**Category**       |[Controls/ Forms/ Graphics/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-graphics-menus__2-59.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/michael-r-brown-text-box-jump__2-1784/archive/master.zip)

### API Declarations

example: <INPUT TYPE="text" NAME="name" VALUE="" SIZE=4 MAXLENGTH=4 onkeyup="NextBox('name',4);">


### Source Code

```
<script LANGUAGE="JavaScript">
<!-- Begin
// Author: Michael Ray Brown
// Email: mrb23@bellsouth.net
//
// This script will allow you to jump from one text box to the next
// when a desired length is reached. There are two input variables
// ObjName --> Name of Text Box
// ObjNum --> Max characters to be typed before jumping
//
// to call this function place the following code to your text box
// instantiaion --> onkeyup="NextBox('text_box_name',value to jump at(int));"
function NextBox(ObjName,ObjNum) {
// 1st example
if (ObjName == "textbox_name here") {
	// move to next text field
	if (ObjNum == 2) {
		if (document.form_name.textbox_name1.value.length == "set value you want to jump at(example='3')) {
			document.form_name.textbox_name2.focus()
			}
		else {
			document.form_name.textbox_name1.focus()
			}
		}
	}
// 2nd example
else if (ObjName == "textbox_name here") {
	// move to next text field
	if (ObjNum == 2) {
		if (document.form_name.textbox_name1.value.length == 2) {
			document.form_name.textbox_name2.focus()
			}
		else {
			document.form_name.textbox_name1.focus()
			}
		}
	}
// 3rd example featuring 4 text boxes
// a good example would be for credit card # input
else if (ObjName == "textbox_name here") {
	// move to next text field
	if (ObjNum == 2) {
		if (document.form_name.textbox_name1.value.length == 4) {
			document.form_name.textbox_name2.focus()
			}
		else {
			document.form_name.textbox_name1.focus()
			}
		}
	else if (ObjNum == 3) {
		if (document.form_name.textbox_name2.value.length == 4) {
			document.form_name.textbox_name3.focus()
			}
		else {
			document.form_name.textbox_name2.focus()
			}
		}
	else if (ObjNum == 4) {
		if (document.form_name.textbox_name3.value.length == 4) {
			document.form_name.textbox_name4.focus()
			}
		else {
			document.form_name.textbox_name3.focus()
			}
		}
	}
}
// End -->
</script>
```

