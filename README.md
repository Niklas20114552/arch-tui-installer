# Arch-TUI-Installer

Arch-TUI-Installer is an Installer for [Archlinux](https://archlinux.org).

It's based on the [Arch Basic Install](https://gitlab.com/sontypiminternet/arch-basic)-Repository on GitLab.

# Please Note!

- There is no Language-Support for other Languages than German
- It's not finished!
### UEFI with QEMU:

Please use the `UEFI x86_64: /usr/share/OVMF/OVMF_CODE_4M.fd` Firmware, not `UEFI`
## Installation with the ISO-File

In the [Releases](https://github.com/Niklas20114552/arch-tui-installer/releases) Tab download the latest ISO File. Then attach the ISO to the VM, burn it to a DVD or copy it to an USB-Stick.
Then type this into the Terminal:

```bash
setup
```
## Manual Installation
### Recommended when key errors occur. (such as Invalid or broken Package (PGP-Signature)
Download the [Archlinux ISO](https://archlinux.org/download/)

In Terminal type this:
```bash
pacman --needed --noconfirm -Sy dialog git
curl -O https://raw.githubusercontent.com/Niklas20114552/arch-tui-installer/main/setup
chmod +x setup
./setup
```

## I found an Issue!

Thank you! Please enable the debug-mode:

Normal installation: Run setup with `setup --debug`

Manual installation: Run setup with `./setup --debug`

Than look for error-messages and write it down. Please report the error in the [Issue](https://github.com/Niklas20114552/arch-tui-installer/issues)-Tab. But first check if it has already been reported
### Upcoming Features:

- Language Support for the Installer.
- Better English for me (Thats an joke!)
