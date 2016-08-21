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

## Find out which CPU core a process is running on

### Method One: testset

```
taskset -c -p <pid>
```

### Method Two: ps

```
ps -o pid,psr,comm -p <pid>
```

The `psr` field indicates which core the process is running on

### Method Thress: top

* Execute `top -p <pid>`.
* Press `f` key, and add "P = Last Used Cpu (SMP)" column to the display.
* Check the "P" column to find out which core the process is running on.

### Method Four: htop

* Execute `htop -p <pid>`.
* Press <F2> key, got to "Columns", add PROCESSOR under "Available Columns".
* The currently used CPU ID of the process will appear under "CPU" column.

---


## ¶ The end
