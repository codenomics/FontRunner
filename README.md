# FontRunner

> This application is built by AI. I made this for myself and I'm uploading it to GitHub for backup and to share in case anyone can get any use out of it. It's pretty specific to my setup and my needs, but if you can get any use out of it, then enjoy.
>
> Use at your own risk. I offer no warranty or guarantees for this software.

## Download

**Latest version: v1.2** (Oct 8, 2026)

- [FontRunner_v1.2_no-install.zip](https://github.com/codenomics/FontRunner/releases/download/v1.2/FontRunner_v1.2_no-install.zip) - 98 KB
- [FontRunner_v1.2_Setup.exe](https://github.com/codenomics/FontRunner/releases/download/v1.2/FontRunner_v1.2_Setup.exe) - 167 KB
- [FontRunner_v1.2_source.zip](https://github.com/codenomics/FontRunner/releases/download/v1.2/FontRunner_v1.2_source.zip) - 84 KB

What's new in v1.2:

- updater versioning fix**

Older versions are on the [Releases page](https://github.com/codenomics/FontRunner/releases).

## Getting started

### Installer (recommended)

1. Download the file ending in `_Setup.exe` above.
2. Double-click it and click Install. It installs just for you - no admin password needed - and adds Start menu and Desktop shortcuts.
3. To remove it later: Windows Settings > Apps, find FontRunner and click Uninstall.

### No install (portable zip)

1. Download the file ending in `_no-install.zip` above.
2. Right-click it > Extract All, and pick a folder. Don't run it from inside the zip.
3. Open the folder and double-click the app's .exe. Nothing is installed; delete the folder to remove it.

Windows says "Windows protected your PC"? Click More info > Run anyway. It shows that for apps without a paid signing certificate.

## Source code

Want to see how it works, or build it yourself? Download the file ending in `_source.zip` above, extract it and double-click `Build.bat`. It only uses the C# compiler that already comes with Windows, so there is nothing to install.

## More details

```
FONTRUNNER
==========

See the fonts installed on your PC, add new ones, remove the ones you
don't want, and save your own fonts to a zip you can add back later.
It can hide the fonts that came with Windows, so you only see the ones
you added.


GETTING STARTED
---------------
Pick one. Both give you the same app.

OPTION 1 - INSTALLER (recommended)
  Download the file ending in _Setup.exe, double-click it and click Install.
  It installs just for you (no admin password) and adds Start menu and
  Desktop shortcuts. Needs Windows 10 (version 1809 or newer) or Windows 11,
  64-bit.
  To remove it later: Windows Settings > Apps > FontRunner > Uninstall.

OPTION 2 - NO INSTALL (zip)
  1. Download the file ending in _no-install.zip. Right-click it -> Extract
  All... and put the FontRunner folder somewhere it can stay (for example
  Documents). Don't run it from inside the zip.
  2. Double-click FontRunner.exe. Nothing is installed; to remove it, delete
  the folder.

EITHER WAY
  Optional: pin it to Start (right-click it in the Start menu or on the
  desktop -> Pin to Start).

"Windows protected your PC"? Click "More info" -> "Run anyway".
Windows shows that for apps downloaded from the internet that aren't
signed with a paid certificate.


USING IT
--------
The SHOW box picks what the list shows:
  Fonts I installed      - only fonts you (or a program) added
  Windows default fonts  - only the fonts that came with Windows
  All fonts
  Duplicates (3)         - extra copies of a font that is installed twice
  Broken entries (2)     - fonts Windows lists but whose file is gone
  Removed fonts (4)      - fonts you removed earlier (backups you can restore)
  Group: ...             - your own groups (see Groups below)
SEARCH finds fonts by name. SORT puts them A to Z, newest added first,
largest first, or most styles first. PREVIEW TEXT changes the sample line
that is drawn in each font. All of these are remembered.

Each row is one font family. Click a row to tick it (Shift+click ticks a
range, Ctrl+A ticks everything you can see). Double-click a row for a big
preview: the whole alphabet and every style of that font. Use the Smaller
and Bigger buttons there to see it at sizes from 12 to 128 px. The small folder
icon on the row shows the font file in File Explorer.
Fonts that came with Windows have a WINDOWS tag and can't be ticked, so
you can't break Windows by accident.

- Remove selected   takes the ticked fonts out of Windows. You are asked
                    first, and a backup copy of every font is kept in
                    %APPDATA%\FontRunner\Removed (one folder per time).
- Add fonts...      pick font files (.ttf .otf .ttc .otc) or zips. You can
                    also drop files, folders or zips on the window.
                    Fonts are installed just for you - no admin password.
- Export zip...     with nothing ticked: all the fonts you installed go into
                    one zip (in a group: that group's fonts). With some
                    ticked: only those.
                    To get them back (on this PC or another), use Add fonts
                    and pick that zip.
- Groups            named sets of fonts, like "Wedding fonts". Tick fonts,
                    click Groups, and add them to a group (or make a new
                    one). Pick the group in the SHOW box to see just those
                    fonts; you can export a whole group as a zip. In a
                    group you can also rename it, delete it (the fonts stay
                    installed) or take fonts out of it.
                    Only fonts you installed can be added to a group.

Tidying up
- Restore:      open SHOW -> Removed fonts, tick fonts and click Restore.
                They are installed again from the backup copies. Fonts that
                are installed again drop off that list by themselves.
                To get rid of backups for good, tick them and click
                Delete backups (or press Delete).
- Duplicates:   shows the extra copies. One copy of each font is always
                kept (Windows' own first, then the oldest). Tick the extras
                and click Remove. A backup is kept, as always.
- Broken entries: tick them (Ctrl+A for all) and click Clean up. This only
                clears the empty entries.

Keys: Ctrl+O add, Ctrl+F search, Ctrl+A tick all, Delete remove ticked,
F5 read the fonts again.


GOOD TO KNOW
------------
- Fonts added by FontRunner are installed for your Windows account only.
  Fonts that were installed for all users live in C:\Windows\Fonts;
  removing those makes Windows show its permission (shield) prompt.
- Programs that are already open (Word, Photoshop...) may need a restart to
  notice added or removed fonts.
- If Windows is still using a removed font, FontRunner finishes deleting
  the file the next time it opens.
- Updates: when FontRunner starts it checks GitHub for a newer version (it only
  reads the public release page; nothing is sent). If you used the installer,
  Update now downloads and runs the new installer for you. If you use the
  no-install zip, it opens the download page instead. The Updates button at
  the bottom checks on demand, and can turn the startup check off.
- Settings are kept in %APPDATA%\FontRunner\settings.txt, your groups in
  %APPDATA%\FontRunner\groups.txt.
- If something goes wrong, FontRunner-log.txt next to FontRunner.exe says what.
- To remove FontRunner: delete its folder, plus %APPDATA%\FontRunner (that
  also holds the backup copies of any fonts you removed).
```

