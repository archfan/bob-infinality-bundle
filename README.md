# bob-infinality-bundle

These are SlackBuilds & patches to rebuild some official packages in Slackware Linux,
are in test so be careful with the result in your system.

## infinality-bundle project

*"infinality-bundle is a collection of software utilizing the power of font
rendering offered by infinality patches and fontconfig rules known as
fontconfig-infinality-ultimate."*

*  Project: https://wiki.archlinux.org/index.php/Infinality-bundle+fonts
*  Source code: https://github.com/bohoomil/fontconfig-ultimate

## Using

**Important**: backup `/etc/fonts/` before you install fontconfig and remove any personal
configuration (`~/.fonts.conf`, `~/.fonts.conf.d` or `~/.config/fontconfig`) to avoid any
issue.

1.  Clone this repository

  ```
  root@darkstar:~# git clone https://github.com/archfan/bob-infinality-bundle
  ```

2.  Build, remove and install packages following this order:

    1.  `source/l/freetype`
    2.  `source/x/fontconfig`
    3.  `source/l/cairo`

    Or just execute as root `install.sh`.

## Notes

*  At this moment these SlackBuilds are from and for **slackware64-current**, but they also
   work with **slackware-current**.
*  I tried to make the minimal modificactions to the originals Slackbuilds.
*  There is not need to select a type of font rendering (Windows, Apple or Ubuntu)
   since the *"aim of infinality-bundle is to make use of the vast potential hidden
   in native Linux font rendering back-end"*. This does not mean you can not
   configure some aspects of the font rendering, please check:
   *  `/etc/profile.d/infinality-settings.sh`
   *  `/usr/doc/fontconfig-*/fontconfig-infinality-ultimate`
