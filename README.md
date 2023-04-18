# Useful Linux Commands
This repository stores Linux commands I find very useful in my case. This may help others as well.

## Kill Process By Port Number
This command kills a process bound to a specified port (`<PORT>`). It is recommended to run this command as root via `sudo`. 

```bash
kill $(sudo lsof -t -i:<PORT>)
```
