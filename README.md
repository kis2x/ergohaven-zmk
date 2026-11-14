# OP36 ZMK firmware

ZMK v0.3.0 firmware for the regular Ergohaven Omega Point 36, with the left half
as the central and ZMK Studio enabled over USB.

The GitHub Actions build produces three files in the `firmware` artifact:

- `op36_left-ergohaven-zmk.uf2`
- `op36_right-ergohaven-zmk.uf2`
- `settings_reset-ergohaven-zmk.uf2`

Edit `config/op36.keymap` for the keymap and `config/op36.conf` for keyboard
settings. Push changes or run the build workflow manually to build firmware.
Tagged pushes also publish the firmware through the release workflow.

The settings reset shield comes from ZMK. Flash it to clear saved settings,
including Bluetooth pairings, then flash the normal firmware for that half.

## Usage

Read through the [ZMK Module Creation](https://zmk.dev/docs/development/module-creation) page for details on how to configure this template.

## More Info

For more info on modules, you can read through through the [Zephyr modules page](https://docs.zephyrproject.org/3.5.0/develop/modules.html) and [ZMK's page on using modules](https://zmk.dev/docs/features/modules). [Zephyr's west manifest page](https://docs.zephyrproject.org/3.5.0/develop/west/manifest.html#west-manifests) may also be of use.
