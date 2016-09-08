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

## ¶ The end

