# Tips - Misc

---

## Find out the name of Linux distribution.

```
cat /etc/*release
```

---

## Generate ssh public-private key pair.

```
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## Mount a remote path via ssh

```
sshfs -o idmap=user,allow_other USER@HOST:DIR /MOUNT_POINT
```

issue: [Why doesn't SSHFS let me look into a mounted directory?](http://serverfault.com/questions/294109/why-doesnt-sshfs-let-me-look-into-a-mounted-directory)

---

## ¶ The end

