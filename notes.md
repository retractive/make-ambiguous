# Notes

### A rundown on chrome extensions

#### Architecture
5 components:
* Manifest
* Background Scripts
* UI Elements
* Content Scripts 
* Options Page

_Background Scripts_ are basically event handlers, and trigger/*do* browsery things like open/close tabs

_Content Scripts_ do things to the contents of a website, such as insert/hide things, copy/paste text, change the CSS, etc. For my project, I'll just be using content scripts.
