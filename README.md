<div align="center">

## About TMouse


</div>

### Description

The global object Mouse, which is of type TMouse, contains information about the mouse. The object Mouse has several properties and one method I'll discuss here. For more properties and methods look in the Delphi help file, I will only discuss one method that is only present in TMouse, and not the methods that are derived from TObject.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Emiel Hollander](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/emiel-hollander.md)
**Level**          |Beginner
**User Rating**    |3.7 (11 globes from 3 users)
**Compatibility**  |Delphi 5, Delphi 4, Pre Delphi 4
**Category**       |[Delphi function enhancement](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/delphi-function-enhancement__7-25.md)
**World**          |[Delphi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/delphi.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/emiel-hollander-about-tmouse__7-56/archive/master.zip)





### Source Code

```
<p>But first the properties. To find out if there actually is a mouse present on
the system, use the property MousePresent.
<p>You can use the property Capture to find out which window is currently
capturing the mouse events. This property returns a handle, that you can use to
find out further information about the window. The property is defined like
this: Property Capture: HWND;
<p>The property CursorPos returns a TPoint and contains the position of the
mouse cursor. You can use Mouse.CursorPos.X and Mouse.CursorPos.Y to find out
the exact position of the mouse cursor.
<p>DragImmediate specifies if clicking the mouse button starts a drag event
immediately, or of drag events are delayed until the mouse has moved the number
of pixels specified in the DragTreshold property.
<p>Use DragThreshold to specify the number of pixels that the mouse cursor must
be moved with the left mouse button down in order to cause a drag event.
<p>The property WheelPresent returns a boolean and specifies whether the mouse
has a wheel.
<p>Use the property WheelScrollLines, which returns an integer, to see how many
lines are scrolled if someone turns the mouse wheel.</p>
```

