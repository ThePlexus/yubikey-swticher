# yubikey switcher

Simple udev rule and script to allow switching between Yubikey smartcards 
for GPG use, without needing to clean directories each time

Install
-----
install clean-card-private-keys script in /usr/local/bin 

```
sudo cp clean-card-private-keys /usr/local/bin/clean-card-private-keys
sudo chmod 755 /usr/local/bin/clean-card-private-keys
```

edit 40-yubikey.rules and replace ```CHANGEME`` with your Linux login name

```
sudo cp 40-yubikey.rules /etc/udev/rules.d/40-yubikey.rules
```

Limiations
----------
Not designed for linux systems with multiple users.
