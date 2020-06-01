# winbox-mac

![Downloads count](https://img.shields.io/github/downloads/nrlquaker/winbox-mac/total.svg)

<p align="center">
  <img src="icon.png" width="200">
</p>

winbox-mac is [MikroTik](https://mikrotik.com) Winbox bundled into macOS app with [Wine](https://www.winehq.org). Wine was cleaned up of 32-bit files.
Icon is provided by [Lucas di Lucca](https://github.com/luccaccine). This is not official [MikroTik](https://mikrotik.com) build and is not related to Mikrotik in any way.

<p align="center">
  <img src="screenshot.png" width="650">
</p>

## Installation

Can be easily installed with [Homebrew Cask](https://caskroom.github.io):

```sh
brew cask install nrlquaker-winbox
```

## Update

Recommended way to update is to use [Homebrew Cask](https://caskroom.github.io):
```
brew update
brew cask upgrade nrlquaker-winbox
```

## Command line arguments

You can pass command line arguments as follow:

```
open /Applications/Winbox-mac.app --args ip login password
```

## Retina mode

After added support for HiDPI displays in `winbox 3.21` now its posible to [enable retina mode](retina_mode/RETINA.md). It has some [issues](https://forum.mikrotik.com/viewtopic.php?f=21&t=157150) now, thats why its not enabled by default.

## Note

To properly import/export addresses you have to run `Winbox-mac.app/Contents/MacOS/startwine` from CLI or add `/bin/bash` to Security & Privacy → Privacy → Full Disk Access. To be able to see hidden files in file choosing dialog press <kbd>Cmd</kbd> + <kbd>Shift</kbd> + <kbd>.</kbd>.

## Reporting bugs

Please make sure that you are using [bug report template](https://github.com/nrlquaker/winbox-mac/issues/new?assignees=nrlquaker&labels=&template=bug_report.md&title=) and checklist is complete. Otherwise it may be closed without review.

## Contributions are welcomed

If you like this project and you find it useful help me to improve it. First of all check if there are some [help needed issues](https://github.com/nrlquaker/winbox-mac/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22). Or you can improve code or documentation.

## Version

Current version is based on [Winbox 3.24](https://download.mikrotik.com/winbox/3.24/winbox64.exe).
Wine version is `5.1 staging`.

Please check [versioning](VERSIONING.md) for versioning scheme explanation.

## Changelog

There are two changelogs in this project. [One](CHANGELOG.md) related to `Winbox-mac`, the [other one](CHANGELOG_WINBOX.md) is for original `Winbox`.

## License

winbox-mac is released under the [MIT License](https://github.com/nrlquaker/winbox-mac/blob/master/LICENSE)
