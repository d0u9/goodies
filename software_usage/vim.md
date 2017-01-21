# Vim

Vim  is  a text editor that is upwards compatible to Vi.  It can be used to edit all kinds of plain text.   It  is  especially useful for editing programs.

---

## Execute last macro

Press `@``@`

---

## Scroll synchronously

```
:set scb
```

or

```
:set scrollbind
```

---

## Open files in split screen

```
vim -O file1 [file2] [file3] ...
```

---

## Start in diff mode.

There should be two, three or four file name arguments.  Vim will open all the files  and  show differences between them.

```
vim -d file` [file2] [file3] ...
```

---

## Mark the current window part of the diff window

Normally, you need to mark two or more files...

```
:diffthis
```

## Mark all window part of the diff window

```
:windo :diffthis
```

## Get the name of the current file

Register `%` contails the name of the current file, and register `#` contains
the name of the alternate file. These registers allow the name of the current
or alternate files to be displayed or inserted.

For example, in directory `/abc` the command `vim def/my.txt` would edit file
`/abc/def/my.

## Get the name of the current file

Register `%` contails the name of the current file, and register `#` contains
the name of the alternate file. These registers allow the name of the current
or alternate files to be displayed or inserted.

For example, in directory `/abc` the command `vim def/my.txt` would edit file
`/abc/def/my.txt`.

```
:echo @%                                def/my.txt
:echo expand('%:t')                     my.txt
:echo expand('%:p')                     /abc/def/my.txt
:echo expand('%:p:h')                   /abc/def

:echo expand('%:p:h:t')                 def                 First get the full path with :p(/abc/def/my.txt),
                                                            then get the head of that with :h(/abc/def),
                                                            then get the tail of taht with :t(def)

:echo expand('%:r')                     my
:echo expand('%:e')                     txt
```

The following commands insert lines consisting of the full path of the current
and alternate files into the buffer:

```
:put =expand('%:p')
:put =expand('#:p')
```

---

## ¶ The end


