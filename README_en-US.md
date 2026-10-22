<div align="center">

# ColorOS Porting Project

[简体中文](/README.md)&nbsp;&nbsp;|&nbsp;&nbsp;English

</div>

## About

Automation tools for porting ColorOS / OxygenOS to selected OnePlus and OPPO devices. The repository covers Android 14–17 generations across branches. Compatibility depends on the branch, device, and source ROM combination; this does not mean every combination has been tested. Check the branch, device codename, and ROM builds before starting.

## Target devices

- OnePlus 8 series: OnePlus 8, 8 Pro, 8T, and 9R
- OnePlus 9 series: OnePlus 9, 9 Pro, and 9RT
- OPPO Find X3 and Find X3 Pro

This is the project's target device list, not a complete test matrix for every branch.

## Historical test notes

The versions below are retained from earlier project documentation as historical references. They are not guarantees for the current branch or every device:

- Base ROMs: OnePlus 8T (ColorOS 14.0.0.600), OnePlus 8 (ColorOS IN2010 13.1.190), and OnePlus 8 Pro (ColorOS IN2020 13.1.0.190)
- Port ROMs: OnePlus 12 (ColorOS 14.0.0.800) and OnePlus Ace 3V (ColorOS 14.0.1.621)

Earlier documentation reported working face unlock, under-display fingerprint, camera, NFC, and automatic brightness. It also listed issues with AOD brightness, voice wake-up, power-off charging, and wired headphones. Behavior can vary with the device, branch, and ROM build. Include exact version details when reporting an issue.

## Usage

Run the tools in a Linux environment such as WSL, Ubuntu, or Deepin:

```shell
sudo apt update
sudo apt install git -y
git clone https://github.com/toraidl/coloros_port.git
cd coloros_port
sudo ./setup.sh
sudo ./port.sh /path/to/base-rom /path/to/port-rom
```

Use base and port packages that you are authorized to obtain. Back up important data and verify the target device, partition layout, and flashing method first; mistakes can cause data loss or leave a device unable to boot. Do not upload full ROM packages, keys, device serial numbers, or other personal data in an issue.

## Contributing

- [Contribution guide](CONTRIBUTING.md): information to include in issues and pull requests.
- [Maintenance plan](docs/MAINTENANCE_PLAN.md): planned work on compatibility records, release notes, and automated checks.

## Credits

This project uses parts or all of the following open-source projects. Thanks to their developers (in no particular order):

- [BypassSignCheck](https://github.com/Weverses/BypassSignCheck) by Weverses
- [contextpatch](https://github.com/ColdWindScholar/TIK) by ColdWindScholar
- [fspatch](https://github.com/affggh/fspatch) by affggh
- [gettype](https://github.com/affggh/gettype) by affggh
- [lpunpack](https://github.com/unix3dgforce/lpunpack) by unix3dgforce
- [miui_port](https://github.com/ljc-fight/miui_port) by ljc-fight
