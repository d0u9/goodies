# awk

GNU awk, a pattern scanning and processing language `awk', a program that you can use to select particular records in a file and perform operations upon them.

Gawk is the GNU Project's implementation of the AWK programming language. It conforms to the definition of the language in the POSIX 1003.2 Command Language And Utilities Standard. This version in turn is based on the description in The AWK Programming Language, by Aho, Kernighan, and Weinberger, with the additional features defined in the System V Release 4 version of UNIX awk. Gawk also provides more recent Bell Labs awk extensions, and some GNU-specific extensions.

---

## Comparison Operators

`<some_value> ~ /<pattern>/` true if `some_value` matches `pattern`.
`<some_value> !~ /<pattern>/` true if `some_value` doesn't match `pattern`.

```
last | awk '$1 ~ /doug/{print}'
```

---

## Regular Expression

```
awk '/<pattern>/{print}'
```

---

## Compound Expression

`&&` and `||` refer to as `and` and `or` respectively.

```
ll /dev | awk '(/^l/) || (/^d/){print}'
```

---

## Skip Remaining Patterns and Expressions

`next` command tells **awk** to skip all remaining patterns and expressions that you have provided, but instead read the next input file.

This command helps you to prevent executing time-wasting steps.

```
ll /dev | awk '/^l/{print "link: "$0; next;} /^d/{print "dir: "$0; next;}'
```

The second expression will be skipped if the current line of `ll` is a link file.

## Print the longest line in file

```
awk 'length > max { max=length;maxline=$0 } END { print maxline; }' <file>
```

---

## ¶ The end
