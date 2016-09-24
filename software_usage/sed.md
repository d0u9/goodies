# sed

`Sed` is a stream editor.  A stream editor is used to perform basic text transformations on an input stream (a file or input from a pipeline).  While in some ways similar to an editor which permits scripted edits (such as ed), sed works by  making  only  one pass over the input(s), and is consequently more efficient.  But it is sed's ability to filter text in a pipeline which particularly distinguishes it from other types of editors.

---

## Add a line at the top of a file

```
sed -i '1s/^/line to insert\n/' /path/to/file
```

---

## Print pattern matched line (Same as **grep**)

```
sed -n '/PATTERN/p' /path/to/file
```

---

## ¶ The end


