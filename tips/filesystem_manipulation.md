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

---

## ¶ The end
