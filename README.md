# KF2 Web Admin Grimoire
WIP Killing Floor 2 server mod manager.

## Features

The main purpose of this is to add support for KF2 Magicked Admin in all other game modes other than Survival ( like Endless, Weekly, Zedternal, ect... ). It also adds the following to KF2 Server's web admin panel.

* Wave counter AND Time in Endless mode's game ticker
* Wave counter in Endless mode's rule list
* Difficulty in Endless mode's rule list
* Allows to see the level of players in "Server Info" and "Players"
* Fast navigation buttons to any other server (configure this by modifying the file "header_fastnav.inc" found in /KFGame/Web/ServerAdmin)
* The update of gamesummary goes from 30 seconds to 1 second
* Possibility to click on a player's Steam ID to access their steam profile in "Players"
* Addition of a tooltip for each column in "Players"
* Allows you to modify and apply the changes made to the .css files in the folder /images

### Future

* Custom map installation
* Multi-server navigation
* 

## Requirements

* Git
* Python 3.x

## Usage

Running `gen-patches.sh` will compare the most recent seed commit in this repo with the latest
and generate patches that apply the difference for the files in `Web`. The
patches are output in the `patches` folder.

The generated patches can be copied into the `admin-patcher/patches`
folder to apply them with the admin-patcher or applied manually with `git am`.

## License

Script and ServerAdmin modifications are released under the terms of the MIT license.
Original ServerAdmin files are property of Tripwire Interactive.
