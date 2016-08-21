# ps

`ps` displays information about a selection of the active processes. If you want a repetitive update of the selection and the displayed information, use **top(1)** instead.

---

## check how long a process has been running

```
ps -p <PID> -o etime
```

or

```
ps -p <PID> -o etimes
```

## Show threads in a process

```
ps -p <PID> H
```

You can check more about thread related ooptions in **ps(1)**.

## Find out which CPU core a process is running on.

```
ps -o pid,psr,comm -p <pid>
```

The `psr` field indicates which core the process is running on

---

## ¶ The end

