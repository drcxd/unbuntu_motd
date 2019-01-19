# unbuntu_motd

This is an article describing how to modify the unbuntu MOTD (Message of the Day).

Files related with motd.

1 /etc/motd

This is a classic, static file which no longer exists since Ubuntu LTS 16.04. If created, however, its content still will be displayed in the motd.

2 /var/run/motd.dynamic

This is what is actually shown on login. This file is updated by PAM by running the scripts in /etc/update-motd.d, if any exists.

So there are two methods to modify the motd. First, create the /etc/motd file and add what you want into it, this will be displayed every time you login. Second, add a shell script which generates the content you want to display. This can display some useful information on the fly like temperatrues and the up time.

Some Tools To Generate Fancy Or Useful Text

1 FIGlet: Create text based ASCII art
2 lm-sensors: Get information such as fan speed or temperature.
3 landscape-common: Ubuntu only
4 Banner: ASCII art
5 Boxes: ASCII art
6 lolcat: Make your text has rainbow colors

Reference https://ownyourbits.com/2017/04/05/customize-your-motd-login-message-in-debian-and-ubuntu/
