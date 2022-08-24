# BestGui Intro
# Apologies
I am sorry for not posting for many months, and for not telling you this:  
# BestGui? What's that?
I was making [BestGui](https://github.com/zachyboy12/bestgui), a Python module for easily creating Guis  
with dictionaries and even JSON! 
# BestGui Hello World
So, the starter program is fairly simple:  
```
import sys
sys.path.append('/path/to/bestgui')
import bestgui
app = bestgui.Gui()
layout = [
  [
    {'type': 'text', 'text': 'Hello, World!'}
  ]
]
app.configure(layout)
app.start()

```  
Got it? Save this and run it. Did you notice that unlike TKinter or Kivy or PyQt, you can highlight it?  
And much, much more.  
So, let's explain the code:  
* sys.path.append - Appends the directory to use the modules there
* app = bestgui.Gui - Creates an app
* layout = [[{'type': 'text', 'text': 'Hello, World!'}]] - Sets variable ```layout``` to a layout (I will explain what a layout is later).
* app.configure(layout) - Configures the layout
* app.start - Starts the app

So let's see what a layout is:  
A layout is one big Python list. And the other lists inside the lists are rows, and inside those rows are widgets.  
Time to see a diagram!  
```
layout = [
  [{'type': 'text', 'text': 'This is a column'}]  # Row
]
```  
Get the picture? Let us now go to widgets.  
Widgets are anything in a BestGui Gui, and the Gui itself.  
Look at this for an example:  
```
{'type': 'type here'}
```  
So, you have to specify the widget type.  
