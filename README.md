# Grey Hack Stack

Small utilities for the Grey Hack video game.

## Wi-Fi inventory (v0.1)

Copy `scripts/wifi_inventory.src` into the in-game CodeEditor and build it as `wifi_inventory`. Run `wifi_inventory` or supply an interface name, e.g. `wifi_inventory wlan0`.

The script scans using the game's native API, displays unique scan rows, and writes a snapshot to `wifi_networks.txt` in the current in-game directory. Existing snapshots are overwritten. No password capture, cracking, or connection is performed.

Status: initial implementation; requires in-game runtime testing. Default interface and exact scan row formatting need confirmation against the installed game version.

Reference: https://greyscript.net/api
