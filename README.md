![GitHub downloads](https://img.shields.io/github/downloads/jonelo/jacksum-for-macos/total?color=green)

# Jacksum for macOS

<img width="737" alt="Screenshot 2024-04-27 at 23 26 45" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/b0846070-b61f-4e74-b8bb-5dc3e6c0eaa1">


## Abstract

Jacksum for macOS is an installation program with which you can easily access functions of [Jacksum](https://github.com/jonelo/jacksum) on macOS.
In other words, it adds more than 480 hash algorithms to your Mac and you can use them with different user interfaces to calculate hash values, verify data integrity, and many moree. See the [Jacksum](https://github.com/jonelo/jacksum) page for more info.

The installation program installs

- [Jacksum](https://github.com/jonelo/jacksum) which is the hash engine, it also provides the command line interface (CLI)
- [HashGarten](https://github.com/jonelo/HashGarten) which is a standalone graphical user interface (GUI) for Jacksum
- script glue to call Jacksum and HashGarten from your preferred file manager

See also the [Architeture](https://github.com/jonelo/jacksum/wiki/Architecture) of interaction between those components.


## System Requirements

### Hardware

- Intel Mac (x64) or Apple silicon (aarch64)
- 150 MiB disk space

### Software

- macOS 10.11 (El Capitan) or later, tested up to macOS 14.4.1 (Sonoma)
- A supported file manager (see below)

#### Supported File Managers

File managers that supports The **Apple Script Menu**-Interface are fully supported by this integration program. In adddition to that a few proprietary interfaces are also supported.

> [!TIP]
> If your preferred file manager does not support the Apple Script Menu, nor allow to use any external scripts nor support any plug-ins, chances are high that your file manager supports at least **drag & drop**, so you could use drag & drop to transfer file/directory-paths from your file manager to the HashGarten GUI where you can process data further, e. g. calculate hashes from file/directory-paths.

The following File Managers have been tested successfully to work with Jacksum and HashGarten:

| File Manager                                                                   | Supported Interfaces  | Comment                                                       |
|--------------------------------------------------------------------------------|-----------------------|---------------------------------------------------------------|
| [Finder](https://support.apple.com/guide/mac-help/mchlp2605/mac)               | DnD + Script Menu     | Commercial Software, the standard file manager from Apple     |
| [Fileside](https://www.fileside.app)                                           | DnD + proprietary API | Commercial Software (Trial), [few extra actions required](https://github.com/jonelo/jacksum-for-macos/wiki/Fileside)     |
| [ForkLift 4](https://binarynights.com/)                                        | DnD + proprietary API | Commercial Software (Trial), [few extra actions required](https://github.com/jonelo/jacksum-for-macos/wiki/ForkLift-4) |
| [muCommander](https://www.mucommander.com)                                     | DnD + proprietary API | Free/Libre Open Source Software (GPLv3)                       |
| [Path Finder](https://www.cocoatech.io)                                        | DnD + Script Menu     | Commercial Software                                           |
|  | | |
| [EasyFind](https://www.devontechnologies.com/en/apps/freeware)                 | DnD                   | Freeware                                                      |
| [CRAX Commander](https://crax.soft4u2.com)                                     | DnD                   | Commercial Software (Demo)                                    |
| [Commander One](https://mac.eltima.com/file-manager.html)                      | DnD                   | Commercial Software                                           |
| [Marta](https://marta.sh)                                                      | DnD                   | Freeware                                                      |
| [Nimble Commander](https://magnumbytes.com)                                    | DnD                   | Free/Libre Open Source Software (GPLv3)                       |
| [Transmit](https://panic.com/transmit)                                         | DnD                   | Commercial Software (Trial)                                   |
| [VioletGiraffe FileCommander](https://github.com/VioletGiraffe/file-commander) | DnD                   | Free/Libre Open Source Software (Apache 2.0)                  |


## Installation

#### 1. Download and open the .dmg

Download and open the [.dmg](https://github.com/jonelo/jacksum-for-macos/releases/latest).

#### 2. Open on the .app

Control-click on the app icon, and choose Open from the shortcut menu. Gatekeeper warns you about the app, but gives you the option to bypass its default policy and open the app.

<img width="981" alt="Open the Jacksum for macOS app" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/846dc6b3-28ac-488d-a76d-a6e44eb68657">


Alternatively, you can open a Terminal to bypass the graphical installation program and run the script directly that is bundled with the installer app. Example for Jacksum 3.7.0:

```
% cd /Volumes/Jacksum\ for\ macOS
% ./Jacksum\ 3.7.0\ for\ macOS.app/Contents/Resources/script
```

#### 3. Check results

At the end of the task a summary will tell you what file managers have been found and where Jacksum and HashGarten have been integrated.

<img width="550" alt="After the installation" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/21a49953-3fa3-41a6-bfb4-21bd1e8ef0ef">


## How to use it

### Using HashGarten

Open the Spotlight Search and search for HashGarten or go to Applications and open HashGarten.

<img width="558" alt="Spotlight Search" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/f57c53d2-8fad-41a3-8f65-229c838db8e3">

### Using Finder and the Script Menu

Go to Finder, select files and folders and choose an action from the Jacksum script folder.

<img width="414" alt="Jacksum at the Finder script menu" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/d8d94614-c927-4f5e-97b6-18d4f3bb3e3b">

From here [HashGarten](https://github.com/jonelo/HashGarten) takes over, and you can calculate checksums, CRCs and hash values of the selected files.

### Using Path Finder and the Script Menu

Open Path Finder, select files and folders and choose an action from the Jacksum script folder.

<img width="449" alt="Jacksum at the Path Finder script menu" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/a1c9467c-30ed-450b-846b-cfa2c03a9291">

From here [HashGarten](https://github.com/jonelo/HashGarten) takes over, and you can calculate checksums, CRCs and hash values of the selected files.

### Using muCommander

Open muCommandere, select files and folders, right click and choose an action from the "Open with..." menu.

<img width="578" alt="muCommander menu" src="https://github.com/jonelo/jacksum-for-macos/assets/10409423/2822f49f-7f26-40ab-ae57-233972aa81b1">

From here [HashGarten](https://github.com/jonelo/HashGarten) takes over, and you can calculate checksums, CRCs and hash values of the selected files.

### Using the Command Line Interface (CLI)

Open a Terminal to get full access to the CLI. Now you can use all features that Jacksum provides.

```
% /Applications/HashGarten.app/jacksum
```

For more information see also [Jacksum](https://github.com/jonelo/jacksum)

## How to configure it

### Finder

Open Finder, click on the script menu, and select "Open Scripts Folder", followed by "Open Finder Scripts Folder".
Alternatively hit ⇧⌘G, enter the path to the Finder scripts folder `~/Library/Scripts/Applications/Finder`, and click on the Go button.

Click on `Jacksum 3.7.0`, and remove any .scpt file that you do not want to see.

### Path Finder

Open Path Finder, click on the script menu, and select "Open Scripts Folder", followed by "Open Path Finder Scripts Folder".
Click on `Jacksum 3.7.0`, and remove any .scpt file that you do not want to see.

### muCommander

Modify the content of `~/Library/Preferences/muCommander/commands.xml` to match your needs.

### How to recreate all items again

Just run the Jacksum for macOS.app again.

## How to uninstall it

Open a Terminal and type
```
% rm -rf /Applications/HashGarten.app
% rm -rf ~/Library/Scripts/Applications/Finder/Jacksum*
```

If Path Finder was found during installation type
```
% rm -rf ~/Library/Scripts/Applications/Path\ Finder/Jacksum*
```

If muCommander was found during installation type
```
% rm ~/Library/Preferences/muCommander/commands.xml
% cp ~/Library/Preferences/muCommander/commands.xml.before_jacksum.* ~/Library/Preferences/muCommander/commands.xml
% rm ~/Library/Preferences/muCommander/commands.xml.before_jacksum.*
```


## Developers Notes

### How to create the .app and .dmg

#### 1. Download and install the Platypus command line tool

The .app will be created by the Platypus command line tool. Platypus is a great tool create Mac apps from command line scripts.
Go to https://sveinbjorn.org/platypus, download and open Platypus, select "Settings..." from the Platypus menu and install the command line tool.

#### 2. Clone the sources

Clone or download the sources from the GitHub project:
```
% git clone https://github.com/jonelo/jacksum-for-macos.git
% cd jacksum-for-macos/
```

Note: if you haven't installed git yet, Apple's Install Command Line Developer Tools will install it for you.

#### 3. Build both the .app and the .dmg

Open a Terminal and run
```
% ./bin/make_all.sh
```
That will build the .app and wrap it in a .dmg. You find both the .app and the .dmg in the folder called `./output/`.

#### 4. Open the .dmg and test the .app

```
% open ./output/*.dmg
```

### Interna of the installation app

The core of the Jacksum for macOS.app is a bash script that installs both HashGarten and Jacksum to the Finder's Script Menu (and other file managers it can detect) by creating applescript scripts (in case of Finder and Path Finder), and compiling those on the system during the installation using osacompile.

The installation script requires Mac OS X 10.4 (Tiger) or later to run. The script does not require admin privileges.
Credits: the installer app has been created by [Platypus](https://sveinbjorn.org/platypus), a great app to wrap shell scripts into a macOS app.

Once the script has been compiled by Platypus, the installer app requires macOS 10.11 or later.
The script source can be revealed again by typing
```
% cd /Volumes/Jacksum\ for\ macOS/
% cat ./Jacksum\ 3.7.0\ for\ macOS.app/Contents/Resources/script
```

The source code of the generated and compiled applescripts can be relealed again by opening the .scpt files (located in the appropriate sccript folders) usiing the
Apple Script Editor or osadecompile.


## Further Information

- [https://jacksum.net](https://jacksum.net)
- https://github.com/jonelo/jacksum
- https://github.com/jonelo/jacksum/wiki/Architecture

## Show your support

Please ⭐️ [this repository](https://github.com/jonelo/jacksum-for-macos) if this project helped you!
