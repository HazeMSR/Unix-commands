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

- tree or lstree: Display the structure of the current directory
```
tree
```
