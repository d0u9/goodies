# awk

GNU awk, a pattern scanning and processing language `awk', a program that you can use to select particular records in a file and perform operations upon them.

Gawk is the GNU Project's implementation of the AWK programming language. It conforms to the definition of the language in the POSIX 1003.2 Command Language And Utilities Standard. This version in turn is based on the description in The AWK Programming Language, by Aho, Kernighan, and Weinberger, with the additional features defined in the System V Release 4 version of UNIX awk. Gawk also provides more recent Bell Labs awk extensions, and some GNU-specific extensions.

---

# Comparison Operators

`<some_value> ~ /<pattern>/` true if `some_value` matches `pattern`.
`<some_value> !~ /<pattern>/` true if `some_value` doesn't match `pattern`.

```
last | awk '$1 ~ /doug/{print}'
```

---

## ¶ The end
