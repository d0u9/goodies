# Compress Tools

Compress tools include **zip**, **gzip**, **bzip2** and **xz**.

Also, the archiving utility **tar** acts an important role in bundling a batch of files and dirs.

---

## Extension name and corresponding compress algorithm.

`*.z`           compressed by **compress**.
`*.zip`         compressed by **zip**.
`*.gz`          compressed by **gzip**.
`*.bz2`         compressed by **bzip2**.
`*.xz`          compressed by **xz**.
`*.tar`         archived by **tar**, uncompressed.
`*.tar.gz`      archived by **tar**, compressed via **gzip**.
`*.tar.bz2`     archived by **tar**, compressed via **bzip2**.
`*.tar.xz`      archived by **tar**, compressed via **xz**.

---

## `.zip`, compress one dir to zip file.

```
zip -r [name.zip] [dir]
```

---

## `.zip`, append files to zip file.

```
zip -g [name.zip] [file1 [file2]]
```

---

## `.zip`, extract file to pip (stdout).

```
unzip -p [name.zip] [file1 [file2]]
```

---

## `.zip`, test archive files.

```
unzip -t [name.zip]
```

---

## `.tar.*`, archive and compress files or dirs

```
# For gzip compress algorithm
tar -zcf [name.tar.gz] [file1 [file2 [...]]]

# For bzip2 compress algorithm
tar -jcf [name.tar.bz2] [file1 [file2 [...]]]

# For xz compress algorithm
tar -Jcf [name.tar.xz] [file1 [file2 [...]]]
```

---

## `.tar.*`, decompress an tar file.

```
tar -zxf [name.tar.gz] -C [dest] [file]
tar -jxf [name.tar.bz2] -C [dest] [file]
tar -Jxf [name.tar.xz] -C [dest] [file]
```

If omit the `-C` option, files will be decompress to current dir.
If omit [file], all files will be extraced.

---

## `.tar.*`, other useful options.

```
-p                     extract information about file permissions (default for superuse)
-P                     don't strip leading '/' from file names.
--exclude=PATTERN      exclude files, given as a PATTERN
```

---

## ¶ The end

