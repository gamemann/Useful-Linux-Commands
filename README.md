# Useful Linux Commands
This repository stores Linux commands I find very useful in my case. This may help others as well.

## Kill Process By Port Number
This command kills a process bound to a specified port (`<PORT>`). It is recommended to run this command as root via `sudo`. 

```bash
kill $(sudo lsof -t -i:<PORT>)
```

## Current CPU Clock Speed
This command lists the current clock speed of each CPU in MHz and updates the output every second.

```bash
watch -n 1 'cat /proc/cpuinfo | grep "MHz"'
```
