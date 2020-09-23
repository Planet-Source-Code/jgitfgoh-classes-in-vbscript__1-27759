<div align="center">

## Classes In VBScript


</div>

### Description

This code will allow you to use classes in VBSccript versions 5.0 and higher
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[jgitfgoh](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/jgitfgoh.md)
**Level**          |Advanced
**User Rating**    |3.9 (27 globes from 7 users)
**Compatibility**  |VB Script, ASP \(Active Server Pages\) 
**Category**       |[Object Oriented Programming \(OOP\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/object-oriented-programming-oop__1-47.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/jgitfgoh-classes-in-vbscript__1-27759/archive/master.zip)





### Source Code

```
'Declare and define a class using the Class statement:
Class cls
	'Private variable to store data:
	Private m_Prop1
	'Propety Prop1:
	'Peoperty Let executes when setting the property
	Public Property Let Prop1(ByVal newVal)
		m_Prop1 = newVal
	End Propertya
	'Property Get executes when reading it
	Public Property Get Prop1()
		Prop1 = m_Prop1
	End Property
	'If the type of the property was class type (and not primitive type) we'd use Property Set instead of Property Get. Property Let souldn't change.
	'Property Prop2:
	'Just a public memeber
	'Can't do range-check, or execute code of any kind
	Public Prop2
	'Declare and define methods just as you'd write normal functions:'Method F
	Sub foo(msg)
		MsgBox msg
	End Sub
'End the Class statement
End Class
Sub Main()
	'make o a "New cls", like in VB5/6
	Dim o
	Set o = New cls
	'Call a method
	o.foo "my message!"
	o.Prop1 = "hello"
	o.Prop2 = "world"
	MsgBox o.Prop1 & " " & o.Prop2 & "!"
End Sub
```

