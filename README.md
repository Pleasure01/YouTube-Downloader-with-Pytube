# YouTube-Downloader-with-Pytube

## Project Prerequisites

To implement this project we use basic concept of python, tkinter, pytube library.

- Tkinter is a standard GUI library and it is one of the easiest ways to build a GUI application.
- pytube used for downloading videos from youtube

To install the required modules run pip installer command on the command line:
```
pip install tkinter
Pip install pytube
```
These are the following steps to build youtube video downloader project in python :

- Import libraries
- Create display window
- Create field to enter link
- Create function to start downloading


### 1. Import Libraries
Start the project by importing the required modules.
```
from tkinter import *
from pytube import YouTube
```
In this python project, we import Tkinter and pytube modules.


### 2. Create Display Window
```
root = Tk()
root.geometry('500x300')
root.resizable(0,0)
root.title("DataFlair-youtube video downloader")
```
- Tk() used to initialize tkinter to create display window
- geometry() used to set the window’s width and height
- resizable(0,0) set the fix size of window
- title() used to give the title of window
```
Label(root,text = 'Youtube Video Downloader', font ='arial 20 bold').pack()
```
- Label() widget use to display text that users can’t able to modify.
- root is the name of the window
- text which we display the title of the label
- font in which our text is written
- pack organized widget in block
### 3. Create Field to Enter Link
```
link = StringVar()
Label(root, text = 'Paste Link Here:', font = 'arial 15 bold').place(x= 160 , y = 60)
link_enter = Entry(root, width = 70,textvariable = link).place(x = 32, y = 90)
```
- link is a string type variable that stores the youtube video link that the user enters.
- Entry() widget is used when we want to create an input text field.
- width sets the width of entry widget
- textvariable used to retrieve the value of current text variable to the entry widget
- place() use to place the widget at a specific position
