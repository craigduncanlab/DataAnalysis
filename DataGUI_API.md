# Data GUI Stacks
(c) Craig Duncan 2018-2020

# Java and JavaFX

# Python and some canvas

# Javascript and some canvas

# D3

Apologies for non-attributions.  If they are missing, please contact me.

# Tkinter

Tkinter is a Python binding to the Tk GUI toolkit. It is the standard Python interface to the Tk GUI toolkit, and is Python's de facto standard GUI. Tkinter is included with the standard Microsoft Windows and Mac OS X install of Python.

Refs for following content:

1.	https://wiki.python.org/moin/TkInter

2. 	2005 http://effbot.org/tkinterbook/

The Tkinter module (“Tk interface”) is the standard Python interface to the Tk GUI toolkit from Scriptics (formerly developed by Sun Labs).  Tk performs an API to the Lib for rendering.

The exact link between the TK library, the creation of classes, and the ultimate expression as screen content follows a structure of passing abstracts back down the chain to Tk API's in C and then to XLib.  See https://docs.python.org/2.4/lib/node721.html

There are class commands in Tk that are usually expressed as a class constructor (fred = class) in python's implementation of Tkinter, which Tkinter uses to pass on to Tk.  See https://docs.python.org/2.4/lib/tkinter-basic-mapping.html

The public interface is provided through a number of Python modules. The most important interface module is the Tkinter module itself. To use Tkinter, all you need to do is to import the Tkinter module:

import Tkinter

Or, more often:

from Tkinter import *

The Tkinter module only exports widget classes and associated constants, so you can safely use the from-in form in most cases. If you prefer not to, but still want to save some typing, you can use import-as:

import Tkinter as Tk

from Tkinter import *

root = Tk()

w = Label(root, text="Hello, world!")
w.pack()

root.mainloop()

Some basic steps:
Popular terminology for categories of classes is to call graphic objects subordinate to the TK objects (i.e. tk classes) 'widgets'.  So things like buttons, labels etc are defined as a 'widget' object from the widget class.

## Tk Canvas

root is a TK() object, which is the window with basic functions; the frame object for the canvas. There is only usually one TK object per application (often called 'root').

The .mainloop method on this will create a loop for events and other things for objects within it.
(this can handle user event such as mouse clicks or key presses, but also other events like sizing)

The Label is an object that can hold a text or image object, and it is created with reference to its parent object (e.g. root) [hierarchical canvas ideas, child nodes etc]

The pack property on Label widget handles geometry and sizing (geometry = size to fit).  This attributes need to be set for each widget or it will not be visible.   It is something which is reviewed before everything is sent off to Tk.
Think of this is a layout manager, and the side attribute can be used to set north/east/west/south type layouts.  See https://docs.python.org/2.4/lib/node725.html

see also https://docs.python.org/2.4/lib/node717.html

There are some good examples of using the Canvas widget here:
https://www.python-course.eu/tkinter_canvas.php

Unlike Label, canvas is a flexible, multi-use base class for drawing.  It seems that to draw a grid requires a low-level approach (no higher level 'objects' or sprites?)

These are all fairly basic, introductory examples.  But in a scientific context, there are ways of borrowing from python libraries that have provided a graphics environment suited to specific tasks, like scientific computing, and biostatistics.  [are these ultimately using Tk under the hood?]
	
