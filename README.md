# Overview
Contains a collection of commands and scripts for Linux.

# Hiding GRUB boot loader
```
sudo nano /etc/default/grub
```

Ensure the following lines are present:
```
GRUB_DEFAULT=0
GRUB_TIMEOUT_STYLE=hidden
GRUB_TIMEOUT=1
```

Apply the changes
```
sudo update-grub
sudo reboot
```

