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

## Empty or delete a large file content

```
: > bigfile
```

```
dd if=/dev/null of=bigfile
```

```
truncate -s 0 bigfile
```

## Copy a File to Multiple Directories

```
echo dest_dir1 dest_dir2 | xargs -n 1 cp src_file
```

---

## Mount vfat filesystem with specific charset

```
mount -t vfat /dev/sdax /mnt -o iocharset=utf8
```

---

## ¶ The end
