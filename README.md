# lync-conf-join
Join Microsoft Lync Conference via invite link on Linux.

[Русский](./README.ru.md) | [English](./README.md)

Install steps:
1. First of all you need to setup and configure Pidgin with Sipe plugin. I assume that you have done it already.
2. Copy contents of the *handler* folder somewhere on yor path, e.g. into $HOME/bin/Lync/ and make *lync* executable
```
chmod +x $HOME/bin/Lync/lync
```
3. Copy *lync.desktop* file into $HOME/.local/share/applications/ and ajust your path where files are located from step2.
4. Copy *lync.png* into $HOME/.local/share/icons/ if you want to see icon in your menu(shortcut will be located under Internet category).
5. Choose what mime types do you need(based on the browser type) in *register_mime.sh* and execute it
```
chmod +x register_mime.sh
./register_mime.sh
```
6. Choose your browser folder and follow the instructions in its readme.

# Notes
Google Chrome support was written based on distro Linux Mint 19.2 with Xfce desktop(because I use it now).
If you want to add support of other distros or DE, feel free to open issues with patches attached and they will be accepted.
