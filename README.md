# Pi-hole LCARS Next Generation Theme
LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Based on the original theme but heavily customized and refactored (still WIP).

[![Dashboard](https://i.imgur.com/PXeXZx7.png)](https://imgur.com/PXeXZx7)

[![Settings](https://i.imgur.com/41QmuUW.png)](https://imgur.com/41QmuUW)

[![Adlist](https://i.imgur.com/uKqZMMG.png)](https://imgur.com/uKqZMMG)

## ⚠️ This theme replaces the original blue LCARS theme ⚠️

## Installation
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/vendor/
sudo git clone https://github.com/jacobbates/pi-hole-midnight.git
sudo rm -f lcars.css
sudo cp pi-hole-lcars-next-gen/lcars.css .
sudo rm -rf pi-hole-lcars-next-gen
```

⚠️ Check the trailing " ." on the 3rd line (it's not a typo - it means copy to current directory).

## Uninstall/Revert
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/vendor/
sudo git reset --hard
```

## Thanks to ...
- [RD Webdesign](https://github.com/rdwebdesign) - creator of the original theme
- [LCARS colors](https://codepen.io/Mokurunner/details/wvyKJy)
- [lcars.org.uk](http://www.lcars.org.uk/) - LCARS panels sections
- [Jacob Bates](https://github.com/jacobbates) for this installation process
---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.