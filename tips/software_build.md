# Tips - network management

---

## Print pre-processor and compile flags required to compile the packages on the command line, including flags for all their dependencies.

```
pgk-config --cflags LIB_NAME
```

You may obtain the full list of modules found in the **pgk-config** path.

---

## Print the link flags, e.g. `-lpthread` or `-lncurses`.

```
pkg-config --libs LIB_NAME
```

---

## ¶ The end
