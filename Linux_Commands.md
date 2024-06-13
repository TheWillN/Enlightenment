# Linux Commands

These are commands to navigate and operate within the command-line interface (CLI).  On a desktop machine, open the Terminal application to access the CLI.  

If you are using Windows Subsystem for Linux then access the terminal within VSCode by going to the menu bar and selecting _Terminal_, then _New Terminal_ in the drop down that appears.  

## List command

```ls```

This command lists all of the contents of a directory. There are a couple modifiers that are helpful and used constantly.
```ls -l```
This is a “long” listing which gives more detail.

On most systems this can be entered with the alias:
```ll```

```ls -h```
The “-h” is for human readable.  This is helpful when looking at sizes.

These modifiers can also stack:
```ls -lh```
___

## Change Directory

```cd <directory>```

This command allows you to move around within the directories.  After you display everything with the
```ls```
 command you can then
```cd```
 into a directory of your choice. To go back one directory enter the command:
```cd ..```
___

## Present Working Directory

```pwd```

This command lets you know where you are, to avoid confusion when you are moving around in various directories or have similar file names in multiple places.
___

## Touch

```touch testfile.txt```

The _touch_ command is a way to create a blank file.  
> Use the ```ls``` command to verify it was created.  
___

## Nano

```nano testfile.txt```

_Nano_ is a text editor.  using the ```nano``` command will open the file you specify for editing.  If the file you name does not exist, it will be created.  
___

## Concatenate

```cat testfile.txt```

Shortened to _cat_, you can use the ```cat``` command to display the contents of a file to the CLI.  

Another use is to redirect the output to another file using the greater-than operator.
```cat testfile.txt > otherfile.txt```
___

## Copy

```cp testfile.txt otherfile.txt```

The ```cp``` command copies the entirety of a file to another file.  
___

## Manual

```man touch```

The ```man``` command followed by another command will provide all the options associated with that command.  Press the "q" to quit the man page.  
___

