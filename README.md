# lync-conf-join
Join Microsoft Lync Conference via invite link on Linux.

Install steps:
1. First of all you need to setup and configure Pidgin with Sipe plugin. I assume that you have done it already.
2. Copy contents of the *handler* folder somewhere on yor path, e.g. into $HOME/bin/Lync/ and make *lync* executable
```
chmod +x lync
```
3. Copy *lync.desktop* file into $HOME/.local/share/applications/ and ajust your path where files are located from step2.
4. Choose what mime types do you need(based on the browser type) in *register_mime.sh* and execute it
```
chmod +x register_mime.sh
./register_mime.sh
```
5. Choose your browser folder and follow the instructions in its readme.
