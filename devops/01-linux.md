# Linux commands and scripts

### Linux Boot Process commands

1. Who is PID 1?
```
ps -p 1
```

Question:

Why is PID 1 special?
<br> --> Its the first user space process that runs after kernel mounts the boot root filesystem

2. What services are running?
```
systemctl list-units --type=service
```

3. How long did Linux take to boot?
```
systemd-analyze
```

4. Which services slowed boot?
```
systemd-analyze blame
```

5. Kernel command line
```
cat /proc/cmdline
```

6. Kernel version
```
uname -r
```

8. Kernel logs
```
dmesg | head -50
```

Notice how early boot messages look.

8. Check boot logs
```
journalctl -b
```
