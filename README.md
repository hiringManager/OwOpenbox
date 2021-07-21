# antiXrespin

This is an MX Linux respin of MX 19.2 with quite a few changes and additions

- Link:
https://drive.google.com/file/d/1jEJvE10SENbm-hO_2xvn-O8hx6BgtkJW/view?usp=sharing

![2020 12 08-02 30 22 screenshot](https://user-images.githubusercontent.com/64992493/126489340-9b1c2579-217a-415b-8ff3-232745cb93f8.png)
![Screenshots2020 07 23-00 39 04 screenshot](https://user-images.githubusercontent.com/64992493/126489360-5c089181-83f1-4183-950a-b226b8557e32.png)


### Login
- User: owl
- Password: toor

Light DM: 
+ Default Session == AwesomeWM (Tiling)
+ Openbox Session
+ Fluxbox (in case you need to configure something that I neglected to include.)

If you'd like to use this as your main setup, it's a simple process to copy this config to a new user. 

``` sudo mx-usermanager ```
Go through the menus and - Create New User - Copy user files (from owl to new user).
Reboot and you're done.

### Defaults

+ Init - sysvinit OR systemd (Both are included in MX, and either can be removed)
+ Shell - ZSH/Antigen
+ WM - AwesomeWM (git and default startX) - Openbox
+ Terminal - urxvt
+ File Manager - thunar / ranger

### Goodies

- Try using fzwal, and check out what is included in ~/.colortoys and ~/.scripts

### Configuration 

- Elenapan's dotfiles:
  See her git for hotkeys, or take a look at 
  ~/.config/awesome/keys.lua # Where many (but not all) of the keybindings are set.
  ~/.config/awesome/rc.lua # Where you'll set default apps, and change the MANY themes that they've made available

- owl4ce's dotfiles: Openbox
  Not much to say here, right click and play around with it. Tons of configuration available.

### Changes: 

- Removals
XFCE: To reduce the size of the image I purged XFCE, except for what is needed to keep MX stable. Fluxbox is still there, unmodified. 

- Additions
ZSH added (see .zshrc to remove anything you dislike)
Picom fork from source (rounded corners, xrender combo whatever)
pywal # wal -i ~/.wallpaper/mechanical/ 
obmenu-generator

- Issues:
  Not sure why but if you load Openbox, you need to press meta+Shift+R to reload for elements to pop up. (or right click reload)
  Left some picom source files in ~/ and ~/Documents. You can delete that.




