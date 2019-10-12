#Steps for Google Chrome

1. When running *regiser_mime.sh* you need to choose *lync15* or *lync* protocol(in my case it was lync15).
2. Copy *xdg-open* somewhere on your path, e.g. into *$HOME/bin* and make it executable
```
chmod +x $HOME/bin/xdg-open
```
3. Add your dir where you have copied *xdg-open* into the PATH variable in your shell user profile(I use bash so I add it into *$HOME/.bash_profile*)
```
export PATH="$HOME/bin:$PATH"
```
4. Open any meeting invitation in browser(just by clicking the link in the invitation email) and when you see a popup to run xdg-open click *yes*. If the Pidgin is running the popup conference window should appear.

#Notes
The *xdg-open* was taken from my linux Mint 19.2 Tina. 
As I use Xfce desktop environment I've only pathed then *open_xfce* function. You can see it in the commit history.
If you use another disto and\or another DE then you need to patch this file in similar way (if links are not executed properly via xdg-open).

#Contribution
Feel free to open pull requests if you want to add fixes for others linux distros or DE.
