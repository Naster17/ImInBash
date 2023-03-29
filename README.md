# Menu 📜
- [System Enumeration](#system-enumeration)


## System Enumeration

```bash
# For the case when the host does not have a tools for viewing processes
cat /proc/*/status | grep "Name:\|State:" 
```
``` bash 
# Checking who else is currently in the system was there 
last -999999 | grep "still" 
# View failed login attempts
lastb -10 # most be root
# Files
/var/log/btmp - Failed login attempts
/var/run/utmp - who is currently logged in (current sessions).
/var/log/wtmp - List of all login sessions.
```
