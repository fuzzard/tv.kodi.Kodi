# Kodi Flatpak
Kodi is an award-winning free and open source software media player and
entertainment hub for digital media. Available as a native application for
Android, Linux, BSD, macOS, iOS, tvOS and Windows operating systems, Kodi runs
on most common processor architectures. This repository packages it through
Flatpak.

## Kodi flatpak build notes.
Before building you need to fetch [shared-modules](https://github.com/flathub/shared-modules) first:

```
git submodule update --init --recursive
```

The following binary plugins do not compile, and are excluded:

 * `game.libretro.2048`
 * `game.libretro.mrboom`

## Contributing

The list of binary addons in each branch of Kodi may be found
[here](https://github.com/xbmc/repo-binary-addons/), and dependencies
[here](https://github.com/xbmc/xbmc/tree/master/tools/depends/target). Kodi
releases are found [here](https://github.com/xbmc/xbmc/releases).

You can contribute by updating addons, modules and the Kodi version.
`make update-addons` can help updating existing addons and also list missing ones

