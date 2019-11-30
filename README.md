# mf-installcab
Installcab based Media Foundation workaround for Wine

For 64bit games:
Just set WINEPREFIX and run mf-installcab64.sh like this

`WINEPREFIX="/home/gaben/.local/share/Steam/steamapps/compatdata/883710/pfx" ./mf-installcab64.sh`

Then copy the included `syswow64/mfplat.dll` to the same directory as the `.exe` (e.g. re2.exe)

installcab.py is exactly the same as upstream (https://github.com/tonix64/python-installcab/blob/master/installcab.py)

### Dependencies
- python
- cabextract
- wine

### Known working games:
- Resident Evil 2
- Resident Evil 7
- Darksiders Warmastered Edition
- Devil May Cry 5
