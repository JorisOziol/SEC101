Instructions

    Install Snort :

https://snort.org/downloads

    Install WinPCap:

https://www.winpcap.org/install/default.htm

    Download and replace config file located in C:\Snore\etc\ path:

https://github.com/JorisOziol/SEC101/blob/main/snort.conf

    You can get some nice community rules from here:

https://github.com/thereisnotime/Snort-2-Rules

    Start your terminal as administrator and type:

cd C:\Snort\bin

    Determine your interface with:

snort -W

    Start Snort on 4th (or whatever number yours is) interface:

snort -i 4 -c C:\Snort\etc\snort.conf

Notes

Snort on Windows does not like SO rules - that is why they are disabled.

If Snort can't find blacklists, whitelists and other files - an error will be thrown. They need to be presented, even if empty.

Current files that you must create: C:\Snort\rules\black.list and C:\Snort\rules\white.list. If you want to use different files - you must modify the configuration file manually.

Also the configuration presumes that your installation is C:\Snort, if it is different, then change it manually from the config file.
