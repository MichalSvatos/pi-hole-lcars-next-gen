# Pi-hole LCARS Next Generation Theme

***

LCARS Theme for [Pi-hole](https://github.com/pi-hole/pi-hole) dashboard. Based on the original theme but heavily customized and refactored.

[![Dashboard](https://i.imgur.com/PXeXZx7.png)](https://imgur.com/PXeXZx7)

[![Settings](https://i.imgur.com/41QmuUW.png)](https://imgur.com/41QmuUW)

[![Adlist](https://i.imgur.com/uKqZMMG.png)](https://imgur.com/uKqZMMG)

### ℹ️ This theme replaces the original blue LCARS theme

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

## Docker installation
Run the same commands directly in the container as shown [here](https://github.com/MichalSvatos/pi-hole-lcars-next-gen/issues/1#issuecomment-1372378045).

_Note: I didn't test it myself._

## Changelog
**1.6.0**
- NEW - DISABLE BLOCKING / CUSTOM TIME modal window styled
- FIX - showed icons in the 4 status boxes on dashboard on mobile + hover adjustment
- FIX - added min-height to `.content` to avoid incorrect footer position when TOOLS menu is open
- FIX - Add `color-scheme: dark` to avoid problems with browser's "Force dark mode" option (copy of the commit [7c2ebef](https://github.com/MichalSvatos/AdminLTE/commit/7c2ebef62b4c79844afed24e5b61d698e93618f1) )
- FIX - colored log has actually colors again

**1.5.4**
- FIX - "TOOLS / UPDATE GRAVITY" section alerts (thx [tismofied](https://github.com/tismofied), [issue](https://github.com/MichalSvatos/pi-hole-lcars-next-gen/issues/3))

**1.5.3**
- FIX - Fit all the buttons in the "SYSTEM" section on one line
- NEW - Showing IP address on checkbox hover in "SYSTEM / DNS" section
- NEW - LCARS panels in "SYSTEM / DNS" section
- NEW - LCARS panels in "SYSTEM / SYSTEM" section

**1.5.2**
- FIX - Shorten stats' boxes animation (it was annoyingly long)

**1.5.1**
- FIX - Calendar width, next/prev month arrow

**1.5.0**
- NEW - styling of the datepicker and calendar

**1.4.0**
- NEW - styling of the data tables - checkboxes, buttons, dropdown menus, background colors

**1.3.2**
- FIX - alerts icon and title align
- FIX - filter in "DOMAINS" on one line
- FIX - small refactoring

**1.3.1**
- FIX - position of the update info ("To install updates, run `pihole -up`")

**1.3.0**
- NEW - Redesigned login screen

**1.2.1**
- FIX - drop down menu links
- UPDATE - Docker installation - thanks to [Griffen8280](https://github.com/Griffen8280)

**1.2.0**
- FIX - "HOSTNAME" word hidden
- FIX - collapsed sidebar after new update
- FIX - styling for the new links in the stats boxes
- NEW - whole stats boxes area is clickable

**1.1.4**
- FIX - footer text color (over-refactoring :) )

**1.1.3**
- FIX - Small refactoring (mostly just color variables)

**1.1.2**
- NEW - Visual change of the counter next to the hamburger menu icon
- FIX - Counter in the sidebar (expanded and collapsed) is no longer flipped horizontally and it's visualization is in style of the rest of the design

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

## Star Trek Picard fan?
Check my other theme (WIP)
[![Pi-hole Star Trek Picard LCARS Theme](https://github.com/MichalSvatos/pi-hole-star-trek-picard/raw/main/previews/pi-hole-star-trek-picard-lcars.png)](https://github.com/MichalSvatos/pi-hole-star-trek-picard)

---
### License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
