These scripts allow using SSH over USB to connect to an iDevice. See
https://marcan.st/blog/iphonelinux/usbmuxd/ and
http://iphonedevwiki.net/index.php/SSH_Over_USB for more details.

I have modified tcprelay.py to allow forwarding SSH connections to multiple
devices instead of just one. The device's udid can be specified using the -u
option. If -u isn't supplied, tcprelay.py will use the first device available.

    python tcprelay.py -t 22:5000 -u ddac43f3247126671d2c7c279723cb2f9f93ace1
