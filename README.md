# mf-installcab
Installcab based Media Foundation workaround for Wine

### Known working games:

- Resident Evil 2
- Resident Evil 7
- Darksiders Warmastered Edition
- Devil May Cry 5
- Borderlands 3

Just set WINEPREFIX and run install-mf-64.sh like this

`WINEPREFIX="/dev/brain/wine prefixes can be anywhere/folder" ./install-mf-64.sh`

Steam stores Proton Wine prefixes as <STEAM FOLDER>/steamapps/compatdata/<GAME ID>/pfx

Optionally you can use Proton's Wine instead of your system's Wine. This requires to provide the `-proton` argument and set PROTON like

`PROTON=$HOME/.local/share/Steam/steamapps/common/Proton\ 5.0/ WINEPREFIX="$HOME/.local/share/Steam/steamapps/compatdata/397540/pfx" ./install-mf-64.sh -proton`

Then copy the included mfplat.dll to the same directory as the `.exe` (e.g. re2.exe)

installcab.py is exactly the same as upstream (https://github.com/tonix64/python-installcab/blob/master/installcab.py) (minor some small differences)

### Dependencies
- python
- cabextract
- wine (optional if proton used)
