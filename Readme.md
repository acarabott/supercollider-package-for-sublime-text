# Supercollider package for Sublime Text 2

Forked from geoffroymontel / supercollider-package-for-sublime-text  
https://github.com/geoffroymontel/supercollider-package-for-sublime-text

Tested on OSX Lion and SC3.5 Mainly  
Tested on XP and SC3.5 (only a little...)

## Usage
- Open Sublime Text 2  
- Go to Preferences/Browse Packages  
- Create a SuperCollider directory.  
- Copy and paste all the files from this repository in it.  
- Change Supercollider path in SuperCollider.sublime-settings
- Restart Sublime Text 2
- Tools > Supercollider > Start sclang

## Keybind(Mac)
- Start SCLang: Cmd + Ctrl + s, Cmd + Ctrl + s
- Stop SCLang: Cmd + Ctrl + s, Cmd + Ctrl + p
- Evaluate current line: Ctrl + enter
- Stop all sound(thisProcess.stop;): Ctrl + .
- Open help from current word: Cmd + Ctrl + s, Cmd + Ctrl + h
- Show console: Cmd + Ctrl + s, Cmd + Ctrl + c
- Clear console logs: Cmd + Ctrl + s, Cmd + Ctrl + l

## Keybind(Windows/Linux)
- Start SCLang: Ctrl + Alt + s, Ctrl + Alt + s
- Stop SCLang: Ctrl + Alt + s, Ctrl + Alt + s
- Evaluate current line: Ctrl + enter
- Stop all sound(thisProcess.stop;): Ctrl + .
- Open help from current word: Ctrl + Alt + s, Ctrl + Alt + h
- Show console: Ctrl + Alt + s, Ctrl + Alt + c
- Clear console logs: Ctrl + Alt + s, Ctrl + Alt + l


geoffroymontel / supercollider-package-for-sublime-text  
https://github.com/geoffroymontel/supercollider-package-for-sublime-text

The syntax highlighting comes from RFWatson's SuperCollider TM Bundle  
https://github.com/rfwatson/supercollider-tmbundle

Sublime Text 2  
http://www.sublimetext.com/2

Supercollider  
http://supercollider.sourceforge.net 


## Bugs
* Console not always showing 

## TODO
* Convert snippets to .sublime-snippet
* Dump Node Tree Command / key map
* Server Meter Command / key map
* Open class file command
* Autocomplete 
* Argument hinting
* Enable/Disable post window scrolling

## Changes

* Key commands now only within SuperCollider syntax context
* Key commands brought in line with SC IDE
	* cmd+b - boot default server
	* ctrl+s ctrl+d for Documentation (help)
	* cmd+shift+c for clear post window (old skool SC.app style, cmd+shift+p is used in ST)
	* shift+enter for line evaluation
	* cmd+enter for line/region evaluation
* Changes to key commands
	* ctrl+s ctrl+s to start sclang
	* ctrl+s ctrl+t to stop sclang
* New commands
	* Server Reboot - ctrl+s, ctrl+b
* Evaluating multiple lines when in between brackets
	* Cursor returns to original position
* Evaluating just currently selected text