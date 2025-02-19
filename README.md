how to install sddm
_1: sudo pacman to install sddm:_
`sudo pacman -S sddm`

2: enable sddm via systemctl:
`systemctl enable sddm.service`

_- reboot and then sddm works_

how to put in a custom theme (downloaded)
_first download your desired theme to you download folder_

_1: move your sddm theme to /usr/share/sddm/themes:_
`sudo mv ~/Downloads/<add-your-theme-here> /usr/share/sddm/themes`

_2: go to /default.conf via the follwing path:_
`/usr/lib/sddm/sddm.conf.d/default.conf`

_3: open default.conf in nvim:_
`sudo nvim default.conf`

_4: change theme to you're theme:_
```
[Theme]
Current theme name
Current=
```
**_change to:_**
```
[Theme]
Current theme name
Current=<add-your-theme-here>
```
_quit the file (with wq) and reboot_
_enjoy your new sddm theme_
