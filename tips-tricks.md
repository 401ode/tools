# Tips and Tricks

## Linux Command Line Tricks

### Line-Clearing

- Clean up the line: You can use <kbd>Ctrl+U</kbd> to clear up to the beginning.
- Clean up the line: <kbd>Ctrl+A</kbd> <kbd>Ctrl+K</kbd> to wipe the current line in the terminal
- Cancel the current command/line: <kbd>Ctrl+C</kbd>.
- Recall the deleted command: <kbd>Ctrl+Y</kbd> (then <kbd>Alt+Y</kbd>)
- Go at the beginning of the line: <kbd>Ctrl+A</kbd>
- Go at the end of the line: <kbd>Ctrl+E</kbd>
- Remove the forward words for example, if you are middle of the command: <kbd>Ctrl+K</kbd>
- Remove characters on the left, until the beginning of the word: <kbd>Ctrl+W</kbd>
- To clear your entire command prompt: <kbd>Ctrl + L</kbd>
- Toggle between the start of line and current cursor position: <kbd>Ctrl + XX</kbd>

*[Source for the above.](https://stackoverflow.com/a/16687377/5000626)*

### Finding Stuff
### Where am I? 
- `pwd` will tell you what directory you're currently in. 
- `pushd` tells the operating system "Remember this directory. I'm going to want to come back here." Optionally, you could say `pushd ~` which would store the current directory location, and then take you to your home directory (`~`). 
- `popd` will return you to the directory you just stored. 


#### Files and Things
If you're in a given directory, typing `ls` will give you a list of the non-hidden files in that directory. Hidden files, you say? What's this hacker stuff? Any file that starts with a `.` is a "hidden" file. In your home directory (get there by doing `cd $HOME` or `cd ~`), you may have a file called `.profile`. This stores a bunch of information about your user. Hidden files are everywhere. Things to keep in mind with `ls`: 
- `ls -a` will show all files, including the hidden ones. 
- `ls -l` will show detailed information about the files, like when it was last modified, who owns it, what permissions it has, etc. 
- `ls -lh` will show the filesizes of the file in a human-readable format, like 1.2MB, 3.7K, etc.
- `ls -lah` will do all three, of course. 

Not surprisingly, `find` is the most powerful command to find stuff in Linux. Good things to remember: 
- `find . -type d` - looks in the current directory ( represented by `.`) and finds things of type `d`, which are directories. 
- `find . -name blah` - looks in the current directory for files named blah.

#### Grep(ping)
`grep` is one of the most powerfully badass commands in the world. Literally books have been written about it. But basically it will look, recursively if you want it to, into all the files in a given directory for some Regular Expression (see below) pattern that you define. So if you want to see every `.log` file that has `error` in it, you would run `grep "error" *.log`. Running that in this directory gets you this: 

```bash
user@coolbox /dev/401ode/tools grep error *.md
tips-tricks.md:`grep` is one of the most powerfully badass commands in the world. Literally books have been written about it. But basically it will look, recursively if you want it to, into all the files in a given directory for some Regular Expression (see below) pattern that you define. So if you want to see every `.log` file that has `error` in it, you would run `grep "error" *.log`. Running that in this directory gets you this:

```


## (Reg)ular (Ex)pressions (RegEx)
- `^` - Start of a line
- `$` - End of a line
- `\s` - A Whitespace character. 

**More to come.**