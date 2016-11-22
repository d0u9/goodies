# Tips - filesystem manipulation

---


## Showing file information for a symbolic link, show information for the file the link reference rather taht for the link itself.

```
ls -L
```

---

## Copy file but never follow symbolic links, and preserve the specified attributes of link.

```
cp -d
```

## Auto mount a dir to another when startup.

Add the line below to **/etc/fstab**.

```
/path/to/src/dir    /path/to/dest/dir	none bind
```

## Truncates a file to zero length (i.e. empty a file)

```
: > data.xxx   # File "data.xxx" now empty.
```

Same effect as   cat /dev/null >data.xxx
However, this does not fork a new process, since ":" is a builtin.

---

## ¶ The end
