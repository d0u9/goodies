# Tips

---

## Find pid(s) of process(es) with their name

```
pidof <binary file name>
```

---

## Count the number of threads in a process

### Method One: /proc

```
cat /proc/<pid>/status
```

The `Threads: <N>` field in output indicates how many threads are current running in this process.

### Method Two: ps

```
ps hH -p <pid> | wc -l
```

---


## ¶ The end
