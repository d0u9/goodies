# git

**Git** is a fast, scalable, distributed revision control system with an unusually rich command set that provides both high-level operations and full access to internals.

---

## Conver a normal git repo to bare repo

```
mv repo/.git repo.git
rm -fr repo
cd repo.git
git config --bare core.bare true
```

---

## ¶ The end


