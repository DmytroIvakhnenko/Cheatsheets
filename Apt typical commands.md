# Apt typical commands

- Hold/unhold package from update
`sudo apt-mark hold package-name`
`sudo apt-mark unhold package-name`
- See all installed packages
`apt list --installed`
- See list of updates
`sudo apt update && apt list --upgradable`
- Install local deb packages 
`sudo apt install ./teamviewer_amd64.deb`
