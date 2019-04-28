
# Standard Notes themes

Repository for community contributed themes for [Standard Notes](https://standardnotes.org/).

## Notes

## Themes

### Better Solarized Dark

This theme was forked from [this repository](https://github.com/swalladge/sn-themes) in a quick attempt to package the *official solarized dark theme* as someone who has not yet bought the extended package.
Only the official .css file was used in place of the original theme's .css, and the links were updated to only take resources from this github page.
The .zip package necessary was created by the current .css and .json file, and includes these files only.
- Author: Orestarod
- License: GPLv3
- Sources: <https://github.com/orestarod/sn-themes>
- Install link: <https://raw.githubusercontent.com/orestarod/sn-themes/master/better-solarized-dark/package.json>

![screenshot](./images/solarized-dark-screenshot.png)

### Material Dark

### Other community themes
This theme is similar to the Better Solarized Dark, but using a slightly different color theme and being based off the [Atom Material UI Theme](https://github.com/atom-material/atom-material-ui)

- [s4skia](https://github.com/flowinho/s4skia), light theme for readability on retina displays.
- [Lyons](https://github.com/jamesjlyons/Lyons)
- Author: vantezzen
- License: MIT
- Sources: <https://github.com/vantezzen/sn-theme-material>
- Install link: <https://cdn.jsdelivr.net/gh/vantezzen/sn-theme-material/extension.json>

![screenshot](./images/material-dark-screenshot.png)

### Gruvbox Dark Theme

Theme based on the [gruvbox theme for vim](https://github.com/morhetz/gruvbox)

- Author: christianhans
- License: MIT
- Sources: <https://github.com/christianhans/sn-gruvbox-dark-theme>
- Install link: <https://listed.standardnotes.org/CkWVdPhzvs>

![screenshot](./images/gruvbox-screenshot.png)



## Developing themes

The easiest way to develop a theme is to pick an existing theme that is
close to what you are wanting, and modify it from there. The desktop and web
applications use the css file, which afaik can contain any valid css, including
font imports and such. The mobile app uses the json style file. (todo: find
docs for what other json keys do)


To make a theme installable, follow the instructions at
<https://docs.standardnotes.org/extensions/publishing.html>.  There are some
gotchas. Most should be clear if you see the package.zip file I use for the
solarized theme. I use the package.json for both the extension metadata and the
package.json that is installed with the app and tells sn which file to load.

__TL;DR__

Theme files like this on an _https_ enabled web server:

```
/webroot/path/
             |- mytheme.json
             \- mytheme.zip
```

Distribute install url as `https://your.server/path/to/mytheme.json`.



# License

    Standard Notes themes
    Copyright (C) 2018 Samuel Walladge and contributors

    This program is free software: you can redistribute it and/or modify it
    under the terms of the GNU General Public License as published by the Free
    Software Foundation, either version 3 of the License, or (at your option)
    any later version.

    This program is distributed in the hope that it will be useful, but
    WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
    or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
    for more details.

    You should have received a copy of the GNU General Public License along
    with this program.  If not, see <http://www.gnu.org/licenses/>.
