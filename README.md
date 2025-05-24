![pic](https://github.com/user-attachments/assets/053bbf5e-214d-4f61-b463-ce577f34ff47)

### How to change the keymap?

1. Fork or use this repository as a template https://github.com/Sifan6688/Corne_ble_zmk.
2. Enable Github Actions for your repository.

You have two options on how to configure your desired keymap:

#### Option 1. Keymap Editor

1. Open [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/).
2. Connect it to your Github account and give an access to your repository to Keymap Editor's app.
3. Make changes to your keymap and press `Save` - it will trigger software build. Wait for it to complete.
4. Grab the `firmware.zip` archive.

#### Option 2. Manual

1. Make changes to the [ergonaut_one.keymap](config/ergonaut_one.keymap) file using your favorite text editor.
2. Commit changes to your repository.
3. Go to `Actions` tab in your Github repository, locate the latest build and wait for it to complete.
4. Grab the `firmware.zip` archive

### How to flash the keyboard?

1. Obtain `firmware.zip`
2. Unzip `firmware.zip` - you should have `ergonaut_one_left_studio.uf2` and `ergonaut_one_right_studio.uf2` files
3. Turn off the power for selected halve (move slider to position `OFF`)
4. Connect selected halve to the PC via USB-C cable
5. Press `RESET` button **twice** to enter DFU mode - you should see new USB device in your file manager
6. Copy the corresponding firmware to the root directory of the new USB device
7. Disconnect selected halve from the PC
8. Repeat steps 3-7 for the other halve

### How to pair halves?

1. Turn off the power for both halves (move slider to position `OFF`)
2. Turn on the power for both halves (move slider to position `ON`)
3. Press `RESET` button **once** on both halves **simultaneously**

---------------------05/24/2025---------------------

Adapted to zmk studio. (https://zmk.studio)

ZMK Studio provides runtime update functionality to ZMK powered devices, allowing users to change their keymap layers without flashing new firmware to their keyboards.

To learn more → https://zmk.dev/docs/features/studio.
