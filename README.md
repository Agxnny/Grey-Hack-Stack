# Grey Hack Stack

Small utilities for the Grey Hack video game.

## Wi-Fi inventory (v0.2)

Copy `scripts/wifi_inventory.src` into the in-game CodeEditor and build it as `wifi_inventory`. Run `wifi_inventory` or specify an interface, e.g. `wifi_inventory wlan0`.

Automatically selects the first wlan interface. Displays current networks by descending signal strength and merges records into `wifi_networks.txt` in the current in-game directory, keyed by BSSID. Rediscovered records replace older observations; out-of-range records retain their last observed signal. The original scan-row format is retained, including ESSIDs with spaces. Invalid existing rows cause an exit before writing.

No password capture, cracking, or connection is performed.

Testing: v0.1 scan and file writing confirmed by user. v0.2 pending in-game testing, including empty file reads, sorting and multiple interface formatting.

Reference: https://greyscript.net/api
