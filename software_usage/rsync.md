# rsync

Rsync is a fast and extraordinarily versatile file copying tool. It can copy locally, to/from another host over any remote shell, or to/from a remote rsync daemon. It offers a large number of options that control every aspect of its behavior and permit very flexible specification of the set of files to be copied.

---

# Sync files to remote, and preserve all properties.

```
rsync -azP source user@host:dest_dir
```

use `--delete` option to delete extraneous files from dest dirs.

`-a` option represents archive mode; equals `-rlptgoD`, check **man(1)** for details.

---

## ¶ The end

