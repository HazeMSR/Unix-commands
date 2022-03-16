# Unix-commands
Some basic unix commands

## System information

- uname: Shows device and kernel information.
```
# Shows architecture of the current server
uname -m

# Shows kernel
uname -r

# Shows all the options of the OS
uname -a
```

- man: Manual of any command
```
# Syntax: man [command]
man uname
```

## Directories

- ls: List the files of the current directory:
```
# Normal
ls

# Include hidden files and details
ls -lsa
```

- mkdir: Make a new directory in the current path or another path:
```
# Make a directory named mydir
mkdir mydir

# Make a new directory inside mydir called as mydir2
mkdir mydir/mydir2
```

- cd: Go to the given directory:
```
# Enter to a simple directory
cd mydir
 
# Out of the current directory
cd ../

# Enter to a nested directory
cd mydir/mydir2
```

- tree or lstree: Shows the structure of the current directory
```
tree
```

## Files
- touch: Creates a new file
```
# creates a empty file
touch example.txt
```

- vi: Open the text editor.
Tips.
VI works with Mnemonic commands for example:
-- Press "i" key in order to switch to "Insert" mode.
-- Press "v" key in order to switch to "Visual" mode.
-- Press "ESC" key to exit any mode.
-- Press : key in normal mode in order to input commands like save with the "w" key and "q" key to exit VI.

```

```
