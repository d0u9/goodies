# Tips - text process

---

## Add a line at the top of a file

```
sed -i '1s/^/line to insert\n/' /path/to/file
```

---

## Skip first X characters in a line

```
# Note: replace X with the number of characters you want to skip
cut -c X-
```

---

## Print duplicated lines

```
cat <file> | sort | uniq -d
```

---

## ¶ The end

