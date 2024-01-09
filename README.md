# tob-pwnagotchi
Contains my config.toml file for my pwnagotchi.

Features:
- Inversed display colors (black background)
- Custom kaomoji
- Japanese language & Text
- Various plugins

Plugins:
- Bluetooth tethering to phone (bt-tether)
- Memory/CPU/Temperature monitor (memtemp)
- Blinking power lights (led)
- Automatic positioning tracker (net-pos)
- Quick dictionary attacks on handshakes (quickdic)
- Displays cracked password (display-password)
- Delete incomplete handshakes (aircrackonly)
- Session statistics (session-stats)
- Configure config.toml file through web UI (webcfg)
- Web GPS map of captured handshakes (webgpsmap)
- Download handshakes from web UI (handshakes-dl)

# Usage
Put the file in your pwnagotchi's SD card either by SCP or just directly accessing it (USB to microSD reader, etc.)


## In your pwnagotchi
```
cp /etc/pwnagotchi/config.toml /etc/pwnagotchi/config.toml.bk # Makes backup of original config.toml file
```

## In your PC

#### Using SCP on USB Ethernet
```
git clone https://github.com/andra-putra/tob-pwnagotchi
scp ./tob-pwnagotchi/config.toml user@10.0.0.2 # Enter correct SSH credentials here. I'm assuming 10.0.0.2 if you connect via USB ethernet (check out pwnagotchi wiki) 
```

#### Using normal MicroSD card reader
```
lsblk # Find where your SD card is mounted
git clone https://github.com/andra-putra/tob-pwnagotchi
cp ./tob-pwnagotchi/config.toml /path/to/your/SDcard/etc/pwnagotchi/config.toml # Make sure you replace this with the correct path to your SD card
```
