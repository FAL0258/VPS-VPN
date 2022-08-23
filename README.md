# Setting up VPS
## Webarena
### Instance Setup:
System: Ubuntu 22.04\
No Firewall enabled

### Create Login account:
Press shift when ECS boot menu appears to enter recory mode
And enter the following to create account to sudoer
```
sudo adduser falcon
sudo adduser falcon sudo
```

### Pre-setups:

To enable ssh
```
sudo nano /etc/ssh/sshd_config
```
Find `PasswordAuthentication` line and change to make it ends with yes
```
sudo systemctl restart sshd
```
