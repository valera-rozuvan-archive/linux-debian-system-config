# Connecting to a wifi router

Please refer to [WiFi/HowToUse](https://wiki.debian.org/WiFi/HowToUse) page on Debian wiki.
Specifically the section `wpa_supplicant`.

Once wifi works, you can add additional connections by expanding the file `/etc/network/interfaces`.
For example:

```
iface wlan_home inet dhcp
    wpa-ssid myssid
    wpa-psk secret_passphrase_hash
```

Where `secret_passphrase_hash` is obtained by running the command:

```
$ wpa_passphrase myssid ssid_very_secret_passphrase
```

Establish a connection by running:

```
# ifup wlan0=wlan_home
```

In the above command, `wlan0` is the actual name of your wifi interface. In my case it is `wlp2s0`.
