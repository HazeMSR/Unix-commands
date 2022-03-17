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

- vi: Opens the text editor.
Tips.
VI works with Mnemonic commands for example:
  - Press "i" key in order to switch to "Insert" mode.
  - Press "v" key in order to switch to "Visual" mode.
  - Press "ESC" key to exit any mode.
  - Press : key in normal mode in order to input commands like save with the "w" key and "q" key to exit VI.

```
# First press I, then enter a random text then press ESC and finally press :wq and ENTER key in order to exit and save

vi example.txt

Some random text 1
Some random text 2
Some random text 3
Some random text 4
Some random text 5
Some random text 6


----INSERT----
:wq!
```
- cp: Copy a file or a directory
```
# Syntax: cp original_file destiny_file
cp example.txt example2.txt

# Copying your file to one directory up
cp example.txt ../example3.txt
```

- mv: Move or rename any file or directory
```
# Syntax: mv original_file destiny_file
mv example2.txt another_example.txt

# Moving your file to one directory up
mv another_example.txt ../
```

- rm: Remove any file or directory

```
# Removing a simple file
touch deleteme.txt && rm deleteme.txt

# Removing a directory
mkdir dir1 && rm -R dir1
```

- cat: Shows the content of a file
```
cat example.txt
```

## Permissions

- chmod: Change who can execute, write and read any file or directory
```
# Syntax: chmod [permissions] [file]
# Permissions with Mnemonic. u: user, g: group, o: others, r: read, w: write, x: execute

chmod ugo+rwx example.txt

# Permissions with Octal. 1st position user, 2nd position group, 3rd position others, 4: read, 2: write, 1: execute, 0: no permission.
# You can add any numbers in order for obtain different combination of permissions, for example 7 represents all the permissions.

chmod 740 example.txt
```

- chown: Change the owner of a file or directory
```
# Syntax: chown [user]:[group] file
# If you only want to change the user you don't have to specify the group

chown anotheruser example.txt

# Or specify the group also
chown anotheruser:anothergroup example.txt
```
