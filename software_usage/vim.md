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

---

## ¶ The end


