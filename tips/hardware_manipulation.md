# Tips - hardware manipulation

---

## Determine the filesystem type of a device.

```
# Can get a basic idea of the filesystem structure (can not obtain the precise type name).
fdisk /sdv/sdX -l

# Can detect without mounting.
blkid

# Can detect without mounting.
parted /dev/sdX -l

# Work only for mounted devices.
df -T

# Can detect without mounting.
file -sL /dev/sdXY

```

---

## ¶ The end
