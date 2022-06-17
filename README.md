# Pi-hole LCARS Next Generation Theme
LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Based on the original theme but heavily customized and refactored (still WIP).

[![Dashboard](https://i.imgur.com/PXeXZx7.png)](https://imgur.com/PXeXZx7)

[![Settings](https://i.imgur.com/41QmuUW.png)](https://imgur.com/41QmuUW)

[![Adlist](https://i.imgur.com/uKqZMMG.png)](https://imgur.com/uKqZMMG)

### ℹ️ This theme replaces the original blue LCARS theme
### ℹ️ Installation does not support Docker at this moment

## Installation
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/themes/
sudo git clone https://github.com/MichalSvatos/pi-hole-lcars-next-gen.git
sudo rm -f lcars.css
sudo cp pi-hole-lcars-next-gen/lcars.css .
sudo rm -rf pi-hole-lcars-next-gen
```

⚠️ Check the trailing " ." on the 3rd line (it's not a typo - it means copy to current directory).

## Uninstall/Revert
Type the following commands into SSH, line by line.

```
cd /var/www/html/admin/style/themes/
sudo git reset --hard
```

## Changelog
**1.1.2**
- NEW - Visual change of the counter next to the hamburger menu icon
- FIX - Counter in the sidebar (expanded and collapsed) is no longer flipped horizontaly and it's visualization is in style of the rest of the design

**1.1.1**
- FIX - footer with UPDATE AVAILABLE text is no longer broken
- FIX - spacing of `pre` in messages section
- NEW - minimized sidebar has a centered icons now (thx for a feedback [AuthorShin](https://github.com/AuthorShin))

**1.1.0**
- FIX - input height in TOOLS --> Query lists
- NEW - lcars-ish checkboxes and radios

**1.0.1**
- fix for small black box in the top bar on smaller screens
- polishing of the 2(3) buttons in the right top corner

## Thanks to ...
- [RD Webdesign](https://github.com/rdwebdesign) - creator of the original theme
- [LCARS colors](https://codepen.io/Mokurunner/details/wvyKJy)
- [lcars.org.uk](http://www.lcars.org.uk/) - LCARS panels sections
- [Jacob Bates](https://github.com/jacobbates) for this installation process
---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
