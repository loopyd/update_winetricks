# update_winetricks
A script to update winetricks automatically to the latest git release.  Can help fix some problems from package maintainers who fall behind.

## Installation

Via curl:

```
curl -sL https://raw.githubusercontent.com/loopyd/update_winetricks/master/update_winetricks | sudo bash -
```

## Usage

This script must be run as root.  To update winetricks to the latest version from GitHub:

```
sudo update_winetricks
```

## Adding to cron jobs

Want to recieve updates every day to ensure you always have the latest version ?

Run the following in a terminal:

```
[[ ! -d /etc/cron.daily ]] && sudo mkdir /etc/cron.daily
pushd /etc/cron.daily
	sudo ln -s /usr/bin/update_winetricks update_winetricks
popd
```

## Enjoy!

Thank you!  Winetricks isn't my software, it can be found at [this repository](https://github.com/Winetricks/winetricks)
