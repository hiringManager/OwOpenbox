# antiXrespin

This is an MX Linux respin of MX 19.2 with quite a few changes and additions

User: owl
Password: toor

If you'd like to use this as your main setup, it's a simple process to copy this config to a new user. 

``` sudo mx-usermanager ```
Go through the menus and - Create New User - Copy user files (from owl to new user).
Reboot and you're done.

Shell - ZSH/Antigen
WM - AwesomeWM (git and default startX) - Openbox
Terminal - urxvt
File Manager - thunar / ranger


Elenapan's dotfiles:
  See her git for hotkeys, or take a look at 
  ~/.config/awesome/keys.lua # Where many (but not all) of the keybindings are set.
  ~/.config/awesome/rc.lua # Where you'll set default apps, and change the MANY themes that they've made available

owl4ce's dotfiles: Openbox
  Not much to say here, right click and play around with it. Tons of configuration available.


Changes: 

Removed:
XFCE: To reduce the size of the image I purged XFCE, except for what is needed to keep MX stable. Fluxbox is still there, unmodified. 

ZSH added (see .zshrc to remove anything you dislike)
Picom fork from source (rounded corners, xrender combo whatever)
pywal # wal -i ~/.wallpaper/mechanical/ 
obmenu-generator

Issues:
  Not sure why but if you load Openbox, you need to press meta+Shift+R to reload for elements to pop up. (or right click reload)
  Left some picom source files in ~/ and ~/Documents. You can delete that.




