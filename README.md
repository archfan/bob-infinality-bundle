# Infinality Bundle for Slackware 14.2

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
