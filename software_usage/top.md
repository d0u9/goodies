# top

The `top` program provides a dynamic real-time view of a running system. It can display system summary information as well as a list of processes or threads currently being managed by the Linux kernel. The types of system summary information shown and the types, order and size of information displayed for processes are all user configurable and that configuration can be made persistent across restarts.

---

## Find out which CPU core a process is running on

* Execute `top -p <pid>`.
* Press `f` key, and add "P = Last Used Cpu (SMP)" column to the display.
* Check the "P" column to find out which core the process is running on.

---

## ¶ The end
