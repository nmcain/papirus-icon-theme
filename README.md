<p align="center">
  <img src="https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/preview.png" alt="preview"/>
</p>

<p align="center">
  <img alt="apps" src="https://img.shields.io/badge/apps_icons-5000%2B-5294e2.svg?style=flat-square"/>
  <img alt="actions" src="https://img.shields.io/badge/actions_icons-2000%2B-5294e2.svg?style=flat-square"/>
  <img alt="panel" src="https://img.shields.io/badge/panel_icons-1900%2B-5294e2.svg?style=flat-square"/>
  <img alt="places" src="https://img.shields.io/badge/places_icons-1250%2B-5294e2.svg?style=flat-square"/>
</p>

Papirus is a free and open source SVG icon theme for Linux, based on [Paper Icon Set](https://github.com/snwh/paper-icon-theme) with a lot of new icons and a few extras, like [Hardcode-Tray support](#hardcoded-tray-icons), [KDE colorscheme support](#kde-colorscheme), [Folder Color support](#folders-color), and [others](#extras).

Papirus icon theme is available in four variants:

 - Papirus
 - Papirus Dark
 - Papirus Light
 - ePapirus (for elementary OS and Pantheon Desktop)

## Contents

 - [Installation](#installation)
    - [Ubuntu and derivatives](#ubuntu-and-derivatives)
    - [Debian and derivatives](#debian-and-derivatives)
    - [Papirus Installer](#papirus-installer)
    - [Third-party packages](#third-party-packages)
 - [Hardcoded icons](#hardcoded-icons)
    - [Hardcoded application icons](#hardcoded-application-icons)
    - [Hardcoded tray icons](#hardcoded-tray-icons)
 - [KDE colorscheme](#kde-colorscheme)
 - [Folder's color](#folders-color)
 - [Extras](#extras)
 - [Recommendations](#recommendations)
 - [Manual fixes](#manual-fixes)
 - [Icon request](#icon-request)
 - [Contributing](#contributing)
 - [Donate](#donate)
 - [License](#license)

## Installation

### Ubuntu and derivatives

You can install Papirus from our official [PPA](https://launchpad.net/~papirus/+archive/ubuntu/papirus):

```
sudo add-apt-repository ppa:papirus/papirus
sudo apt-get update
sudo apt-get install papirus-icon-theme
```

or download .deb packages from [here](https://launchpad.net/~papirus/+archive/ubuntu/papirus/+packages?field.name_filter=papirus-icon-theme).

**NOTE:** Now the daily builds of the papirus-icon-themes package are placed in [`ppa:papirus/papirus-dev`](https://launchpad.net/~papirus/+archive/ubuntu/papirus-dev).

### Debian and derivatives

Debian users also can install Papirus from our [PPA](https://launchpad.net/~papirus/+archive/ubuntu/papirus), but the commands will differ:

```
sudo sh -c "echo 'deb http://ppa.launchpad.net/papirus/papirus/ubuntu bionic main' > /etc/apt/sources.list.d/papirus-ppa.list"

sudo apt-get install dirmngr
sudo apt-key adv --recv-keys --keyserver keyserver.ubuntu.com E58A9D36647CAE7F
sudo apt-get update
sudo apt-get install papirus-icon-theme
```

### Papirus Installer

Use the scripts to install the latest version directly from this repo (independently of your distro):

**NOTE:** Use the same script to update icon themes.

#### ROOT directory (recommended)

```
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/install.sh | sh
```

#### HOME directory for GTK

```
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/install.sh | DESTDIR="$HOME/.icons" sh
```

#### HOME directory for KDE

```
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/install.sh | DESTDIR="$HOME/.local/share/icons" sh
```

#### \*BSD systems

```
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/install.sh | env DESTDIR="/usr/local/share/icons" sh
```

**NOTE:** Qt4 apps require `libqt4-svg` to work correctly.

#### Uninstall

```
wget -qO- https://raw.githubusercontent.com/PapirusDevelopmentTeam/papirus-icon-theme/master/uninstall.sh | sh
```

### Third-party packages

Packages listed in this section are third-party packages. If you have a problem or a question, please contact the package maintainer.

Please note that some packages in the list may be outdated, open [Repology](https://repology.org/project/papirus-icon-theme/versions) to find out package versions.

| **Distro**    | **Maintainer**       | **Package**                              |
| :------------ | :------------------- | :--------------------------------------- |
| ALT Linux     | Andrey Cherepanov    | `apt-get install papirus-icon-theme` <sup>[[link](https://packages.altlinux.org/en/Sisyphus/srpms/papirus-icon-theme)]</sup> |
| Arch Linux    | Felix Yan            | `sudo pacman -S papirus-icon-theme` <sup>community</sup> |
| Arch Linux    | Mohammadreza Abdollahzadeh | [papirus-icon-theme-git](https://aur.archlinux.org/packages/papirus-icon-theme-git/) <sup>AUR</sup> |
| Debian 9+     | Yangfl               | `sudo apt install papirus-icon-theme` |
| Fedora 27+    | Robert-André Mauchin | `sudo dnf install papirus-icon-theme` |
| Fedora        | Dirk Davidis         | [papirus-icon-theme](https://copr.fedorainfracloud.org/coprs/dirkdavidis/papirus-icon-theme/) <sup>copr</sup> |
| FreeBSD       | Hiroki Tagato        | [papirus-icon-theme](https://www.freshports.org/x11-themes/papirus-icon-theme) <sup>freshports</sup> |
| NetBSD        | Nia Alarie           | [papirus-icon-theme](http://pkgsrc.se/graphics/papirus-icon-theme) <sup>pkgsrc</sup> |
| NixOS         | Nixpkgs Contributors | `nix-env -iA nixos.papirus-icon-theme` |
| openSUSE      | Konstantin Voinov    | [papirus-icon-theme](https://software.opensuse.org/download.html?project=home:kill_it&package=papirus-icon-theme) <sup>OBS [[link](https://build.opensuse.org/package/show/home:kill_it/papirus-icon-theme)]</sub> |
| openSUSE      | Matthias Eliasson    | [papirus-icon-theme](https://software.opensuse.org/package/papirus-icon-theme) <sup>official</sup> |
| ROSA Linux    | Vladimir Penchikov   | `sudo urpmi papirus-icon-theme` |
| Solus         | Joshua Strobl        | `sudo eopkg it papirus-icon-theme` |
| Ubuntu 18.04+ | Yangfl               | `sudo apt install papirus-icon-theme` |
| Void Linux    | Giuseppe Fierro      | `sudo xbps-install -S papirus-icon-theme` |

**NOTE:** If you are a maintainer and want to be in the list, please create an issue or make a pull request.

## Hardcoded icons

Some software uses an absolute path instead of the icon name in a .desktop file or in the source code which makes them unthemable.

### Hardcoded application icons

To deal with hardcoded application icons we recommend using [hardcode-fixer](https://github.com/Foggalong/hardcode-fixer). Papirus supports most of the applications in the [list](https://github.com/Foggalong/hardcode-fixer/blob/master/tofix.csv). If [hardcode-fixer](https://github.com/Foggalong/hardcode-fixer) doesn't support your favorite app yet, please open an issue [here](https://github.com/Foggalong/hardcode-fixer/issues) or edit your .desktop file manually.

### Hardcoded tray icons

To fix hardcoded tray icons Papirus supports [Hardcode-Tray](https://github.com/bil-elmoussaoui/Hardcode-Tray) script. A list of supported applications is available [here](https://github.com/bil-elmoussaoui/Hardcode-Tray/tree/master/data/database).

**NOTE:** To get Papirus to work right with Hardcode-Tray, use the hardcode-tray option `--conversion-tool RSVGConvert`:

```
sudo -E hardcode-tray --conversion-tool RSVGConvert --size 22 --theme Papirus
```

**Size recommendations:**

- Unity 22px
- KDE 22px
- GNOME 22px ([see](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme#manual-fixes) for more info)
- XFCE 22px ([see](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme#manual-fixes) for more info)
- Pantheon 24px
- Cinnamon 16px


![hardcode-tray](https://i.imgur.com/6hFm6aj.png)

**BUG on KDE with libappindicator**: Some applications have wrong rendering by default on KDE. For solve this run application with Unity environment option.

For example:

```
XDG_CURRENT_DESKTOP=Unity wire-desktop
```

See more info [here](https://bugs.kde.org/show_bug.cgi?id=366062) and please vote for this bug.

## KDE colorscheme

Support for monochrome icons for KDE colorscheme is now available:
- Papirus - for dark plasma theme & light color scheme
- Papirus Dark - for dark plasma theme & color scheme
- Papirus Light - for light plasma theme & color scheme

![kde-color-scheme](https://i.imgur.com/oM1qhQH.png)

**NOTE:** Non-KDE apps don't support KDE colorscheme on the system tray, but you can replace color manually.

## Folder's color

Papirus has [Folder Color](http://foldercolor.tuxfamily.org/) v0.0.80+ support that allows you to change a color of a folder.

Available colors:

![Folder Color Preview](https://i.imgur.com/jP3mRci.png)

For KDE, colors of individual folders can be changed using [dolphin-folder-color](https://github.com/audoban/dolphin-folder-color).

Also, you can use our [papirus-folders](https://github.com/PapirusDevelopmentTeam/papirus-folders) script to apply the color of folders system-wide.

## Extras

- [Papirus theme for LibreOffice](https://github.com/PapirusDevelopmentTeam/papirus-libreoffice-theme)
- [Papirus themes for FileZilla](https://github.com/PapirusDevelopmentTeam/papirus-filezilla-themes)
- [Papirus theme for SMPlayer](https://github.com/PapirusDevelopmentTeam/papirus-smplayer-theme)
- [Papirus themes for Claws Mail](https://github.com/PapirusDevelopmentTeam/papirus-claws-mail-theme)
- [Papirus themes for Thunderbird](https://github.com/PapirusDevelopmentTeam/thunderbird-theme-papirus)
- [Papirus theme for aMule](https://github.com/PapirusDevelopmentTeam/papirus-amule-theme)

## Recommendations

- Recommended use Papirus icons alongside one of the following GTK themes:
  - [Adapta theme](https://github.com/adapta-project/adapta-gtk-theme)
  - [Arc theme](https://github.com/NicoHood/arc-theme)
  - [Materia theme](https://github.com/nana-4/materia-theme)
- For KDE, our recommendation is:
  - [Adapta KDE](https://github.com/PapirusDevelopmentTeam/adapta-kde)
  - [Arc KDE](https://github.com/PapirusDevelopmentTeam/arc-kde)
  - [Materia KDE](https://github.com/PapirusDevelopmentTeam/materia-kde)

## Manual fixes

<details>
<summary>For Cinnamon users</summary>

For Cinnamon users who want to use Papirus icon theme with [Arc theme](https://github.com/NicoHood/arc-theme) we recommend fix color icons on panel:

```
sudo sed -i.orig 's/white/#d3dae3/g' /usr/share/themes/Arc-Dark/cinnamon/cinnamon.css
```

![Cinnamon Arc-Dark theme fix](https://i.imgur.com/XXejgtD.png)

To deal with blurred panel icons, increase the panel size up to 30px in `Systems Settings` → `Panel` (see [screenshot](https://i.imgur.com/oToRBYv.png)).
</details>

<details>
<summary>For GNOME Shell users</summary>

For GNOME users who want use Papirus icon theme with [Arc theme](https://github.com/NicoHood/arc-theme), we recommend change icons color for panel:

```
sudo sed -i.orig 's/white/#d3dae3/g' /usr/share/themes/Arc-Dark/gnome-shell/gnome-shell.css
```

Translucent panel on Adapta Nokto Gnome Shell theme:

```
sudo sed -i.orig '/panel:overview/ s/rgba(19, 25, 28, 0.01)/rgba(19, 25, 28, 0.7)/g' /usr/share/themes/Adapta-Nokto/gnome-shell/gnome-shell.css
```

Also, we recommend install the following extensions:

- [(K)StatusNotifierItem/AppIndicator Support](https://extensions.gnome.org/extension/615/appindicator-support/) **¹** — This extension integrates AppIndicators. The patched version of [sni-qt](https://github.com/bilelmoussaoui/sni-qt) for [Hardcode-Tray](https://github.com/bilelmoussaoui/Hardcode-Tray) doesn't work without it.
- [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) **¹**
- [No Symbolic Icons](https://extensions.gnome.org/extension/1304/no-symbolic-icons/)
- [Status Area Horizontal Spacing](https://extensions.gnome.org/extension/355/status-area-horizontal-spacing/)

**¹** On Ubuntu 18.04+ it is pre-installed.
</details>

<details>
<summary>For Unity users</summary>

For Unity users, we recommend installing patched [Notify-OSD](https://launchpad.net/~leolik/+archive/ubuntu/leolik) and changing the icon size to 33px.

*~/.notify-osd* file:

```
slot-allocation = dynamic
bubble-expire-timeout = 10sec
bubble-vertical-gap = 10px
bubble-horizontal-gap = 10px
bubble-corner-radius = 24px
bubble-icon-size = 33px
bubble-gauge-size = 6px
bubble-width = 240px
bubble-background-color = 2f343f
bubble-background-opacity = 95%
text-margin-size = 10px
text-title-size = 100%
text-title-weight = bold
text-title-color = adb7bf
text-title-opacity = 100%
text-body-size = 90%
text-body-weight = normal
text-body-color = eaeaea
text-body-opacity = 100%
text-shadow-opacity = 50%
location = 1
bubble-prevent-fade = 1
bubble-close-on-click = 1
bubble-as-desktop-bg = 0
```

![notify-fix](https://i.imgur.com/hjTpvca.png)

Also, you can change [Unity launcher icon](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme/tree/master/extra/unity) and [unity-tweak-tool icons](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme/tree/master/extra/unity-tweak-tool). Look into the extra folder in the icon theme.
</details>

<details>
<summary>For Xfce users</summary>

Here are a few recommendations for Xfce users.

#### Thunar File Manager

Go to `Edit` → `Preferences...`. Click on `Side Pane` tab. Under `Side Pane`, look for `Icon Size` and set to `Very Small`.

![thunar-prefecences](https://i.imgur.com/Iu1TIEa.png)

#### Notification Area

Go to `Settings Manager` → `Panel` → `Items` tab. Select `Notification Area` item and click on `Edit currently selected item` button. Under `Appearance` set the following options:

- Set `Maximum icon size (px)` to `24`
- Uncheck `Show frame`

![xfce4-notification-area](https://i.imgur.com/MopCZBZ.png)
</details>

<details>
<summary>For elementary/Pantheon users</summary>

With light wallpaper, we recommend disable `use-transparency` option on wingpanel:

```
gsettings set org.pantheon.desktop.wingpanel use-transparency false
```

</details>

## Icon request

- Application name
- Icon name (see desktop-file option **Icon** on `/usr/share/applications`)
- Original icon image
- Small description and/or a link to the official webpage

**NOTE**: We do NOT support Windows/Wine/Crossover or other NOT native Linux-apps. This also applies to discontinued projects!!

## Contributing

We welcome user contributions. If you don't know where to start, we've compiled a list of things we would like to see in your pull request:

- new icons for missing applications
- symbolic links to an existing icon
- resolving open issues
- spelling, grammar, phrasing
- improvements to our scripts

Inside [tools/work](tools/work) you will find a step-by-step guide, an environment, and tools that will help you:

- [create a new icon](tools/work#create-a-new-icon) from template
- [make a symlink to an existing icon](tools/work#make-symlinks-to-an-existing-icon)
- [edit an existing icon](tools/work#edit-an-existing-icon)
- convert your icon to all variants of the theme

We are waiting for your pull requests and would love to see this icon theme become as complete as possible.

## Donate

You can support this open source project by making a voluntary payment:

- Patreon: https://www.patreon.com/varlesh
- PayPal: https://www.paypal.me/varlesh

## License

Papirus icon theme distributed under the terms of the GNU General Public License, version 3. See the [`LICENSE`](LICENSE) file for details.
