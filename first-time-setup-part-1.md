# First time setup: part 1

1. Install `aptitude`:

```
apt-get install aptitude apt-transport-https
```

2. Do the usual `update && upgrade`:

```
aptitude update
aptitude upgrade
```

3. Install `sudo`:

```
aptitude install sudo
```

4. Configure running sudo without a password.
See [how to do this](https://askubuntu.com/questions/147241/execute-sudo-without-password).

5. Install system necessities:

```
sudo aptitude install \
  firmware-linux-free firmware-brcm80211 firmware-iwlwifi \
  alsa-firmware-loaders alsa-utils alsa-tools upower mesa-utils
```

6. Install X.org & friends:

```
sudo aptitude install \
  xorg xserver-xorg-core xserver-xorg-input-all xserver-xorg-video-all openbox \
  openbox-menu obconf feh gmrun menu terminator wpasupplicant firefox-esr \
  xscreensaver xscreensaver-data xscreensaver-data-extra xscreensaver-gl \
  xscreensaver-gl-extra
```

7. Install some useful utilities:

```
sudo aptitude install git pv pavucontrol zip unzip rar unrar
```

8. Reboot the system.
