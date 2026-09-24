- [Chinese](README_CN.md)
- [English](README.md)

# Update List

- 2024/12/21
  1. Added support for zmk-studio (just refresh the left hand to use).
- 2024/10/24
  1. Modified power supply mode to reduce power consumption.
  2. Fixed the automatic shut-off feature for RGB power supply.

> If your keyboard was updated before October 24, please update to the latest firmware.
> 
---
# Contact Me

For 3D printed model files or any issues and malfunctions with the keyboard, please contact 380465425@qq.com

# Updating the Keyboard Config

This repo is a standard ZMK user config, built via the GitHub Actions workflow in `.github/workflows/build.yml`.

1. Edit the keymap/config in `config/` (e.g. `config/eyelash_sofle.keymap` for key bindings, `config/eyelash_sofle.conf` for feature flags).
2. Commit and push to GitHub (or open a PR and merge it). The push triggers the `Build ZMK firmware` Action, which builds a `.uf2` firmware file for each board/shield listed in `build.yaml`.
3. Once the Action finishes, open its run under the **Actions** tab and download the `firmware` artifact (a zip containing the `.uf2` files).
4. Flash each half: put the half into bootloader mode (double-tap the reset button), then drag-and-drop the matching `.uf2` file onto the drive that appears (e.g. `eyelash_sofle_left-...uf2` for the left half). Flash both halves separately.

See the ZMK docs for the full flow: [Flashing Firmware](https://zmk.dev/docs/user-setup#flashing-firmware) and [Customizing / editing the keymap](https://zmk.dev/docs/customization).

# Sofle Keymap


<img src="keymap-drawer/eyelash_sofle.svg" >

