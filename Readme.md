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


## TODO
* Clicking error message with "line xxx" takes you to that line in file.
* Open class file should go to symbols
* Quit server on quitting ST2
* Help command without selection should just open Help main page
* Flaggable scrolling on / off of post window
* Need to restart ST if sclang crashes, because variables are not None
* Class(Class) doesn't recognise inner class, e.g. FFT(LocalBuf)
* ST bracket expansion expands (to here)(from here) if there is no return or semi colon
* Find all implementations of
* make sure all commands are in menu
* Maintain focus on ST2 when executing GUI code?
* Consider using separate window for output, can't search terminal
* Convert snippets to .sublime-snippet
* Dump Node Tree Command / key map
* Server Meter Command / key map
* Autocomplete 
* Argument hinting
* Enable/Disable post window scrolling
* "variable: ".post; variable.postln; snippet
* use sclang_process.communicate rather than stdin.write http://docs.python.org/2/library/subprocess.html#subprocess.Popen.stdin
* could open_class_command be done with .communicate rather than .unixCmd, safer?

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
* Simplified parameter syntax matching
	* Pro: New lines work
	* Con: No hinting for invalid values