
2024-09-28 06:33

Tags: [[Arch]] | 

### Overview
List of steps for pairing to bluetooth in arch

### Steps
1. a. `systemctl enable bluethooth.service`
1. b. `systemctl start bluethooth.service`

2. `bluetoothctl`
3. `power on`
4. `agent on`
5. `scan on`
6. Look for the mac address of the device you need:
    - `pair <mac-address>`
7. `connect <mac-address>`

### Source Material
- [Reddit comment](https://www.reddit.com/r/archlinux/comments/13cr6mj/how_to_setup_bluetooth_service_on_arch_linux/)
- [AUR Link](https://wiki.archlinux.org/title/Bluetooth)


### References
- [[]]

