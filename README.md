# OwOpenbox (because UwUbuntu was taken)

This is an MX Linux respin of MX 19.4 with quite a few changes and additions.  
(Goodbye XFCE, didn't want you anyway.)
(Conky, more like 'Gone-ky')

- Version 1.0 - Download: https://drive.google.com/file/d/1jEJvE10SENbm-hO_2xvn-O8hx6BgtkJW/view?usp=sharing
- Version 1.1 - Download:  https://drive.google.com/file/d/1Xq_uhQ-lDWCzQ8BGV4cQvS2UWa5TV_rO/view?usp=sharing

- Included dotfiles, heroes, and dependencies. 
 https://github.com/owl4ce/dotfiles
 https://github.com/elenapan/dotfiles
- *Not included*
- ANYTHING ANIME RELATED EXCEPT FOR WHAT CAME IN OWL'S DOTFILES

![2020 12 08-02 30 22 screenshot](https://user-images.githubusercontent.com/64992493/126489340-9b1c2579-217a-415b-8ff3-232745cb93f8.png)
![2021 07 23-00 19 14 screenshot](https://user-images.githubusercontent.com/64992493/126741984-b924d1e1-48e2-411c-a534-65134ebe2b42.png)
![2021 07 23-00 38 58 screenshot](https://user-images.githubusercontent.com/64992493/126742353-04c95a32-8899-430d-a9cb-8ce59e70804f.png)

# Version 1.1

![image](https://user-images.githubusercontent.com/64992493/126877164-85b150ce-a39f-49e5-ada9-58226cc0f064.png)

### Login
- User: owl
- Password: toor

Light DM: 
+ Default Session == AwesomeWM (Tiling)
+ Openbox Session
+ Fluxbox (in case you need to configure something that I neglected to include.)

To install on your rig just run 'sudo minstall' for the guided install.

If you'd like to use this as your main setup, it's a simple process to copy this config to a new user. 

``` sudo mx-usermanager ```
Go through the menus and - Create New User - Copy user files (from owl to new user).
Reboot and you're done.

### Defaults

+ Init - sysvinit OR systemd (Both are included in MX, and either can be removed)
+ Shell - ZSH/Antigen
+ WM - AwesomeWM (git and default startX) - Openbox
+ Terminal - urxvt/xfce4-terminal/kitty
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
  - Not sure why but if you load Openbox, you need to press meta+Shift+R to reload for elements to pop up. (or right click reload)
  - Left some picom source files in ~/ and ~/Documents. You can delete them.
  - // Replaced with xfce4-terminal in Awesome // urxvt breaks when resizing with Ctrl+Shift+Plus. Can't fix this without editing the config.
## Future Updates
- Add puppy Linux 'woof' at login because it's adorable
- Make theme-switcher for Elena's dots
- Find that gradient generator git and add it
- ImageGoNord maybe? idk seems bloat
- Make rofi quit being fucking annoying
- Add in Doom Emacs, but find a way to get image size WAY down.
- Patch cacaview or whatever into vifm/ranger. (partially done)
- purge picom and properly make a package for it
- find make dependencies for awesome and picom to cut down iso size.
- check sddm deps and switch to it or slim. maybe tui-dm but that may prove too hacky
- Purge either sysvinit or systemd to get iso down to <2GB
- Make fluxbox mildly sexier even though I don't exactly want it listed in lightDM
- Add in tile script for openbox.
- Fix network manager erroring on the horizontal layout. # mv ~/.config/openbox/exec/network elsewhere for now. 
- I want that awesome.spawn(keybinds) Meta+S thingy from the main branch. What's up with that, and can I just plug it back in? 

## New Additions July 24
- cacaview now usable for ascii waifus # cacaview /path/to/waifu
- XFCE4-Terminal main now due to urxvt breakage. 
- Purged Librioffice/memeOfficeSuite and knocked ISO down by like 500 MB
- Removed default settings for Awesome that I'd setup because people hate borders 'cept me
- terminal now loads your last pywal / fzwal colors @exec
- bpytop added for swagger
- Added in cutechonky script to make your widgets feel more cute and chonky
- Added in 'cutefetch' an alternative to bunnyfetch with animals that are more kawaii
- purged nixpkgs I added out of laziness
