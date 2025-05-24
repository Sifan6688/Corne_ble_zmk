![pic](https://github.com/user-attachments/assets/053bbf5e-214d-4f61-b463-ce577f34ff47)

How to change the keymap?
Fork or use this repository as a template https://github.com/ergonautkb/one-zmk-config.
Enable Github Actions for your repository.
You have two options on how to configure your desired keymap:

Option 1. Keymap Editor
Open Keymap Editor.
Connect it to your Github account and give an access to your repository to Keymap Editor's app.
Make changes to your keymap and press - it will trigger software build. Wait for it to complete.Save
Grab the archive.firmware.zip
Option 2. Manual
Make changes to the ergonaut_one.keymap file using your favorite text editor.
Commit changes to your repository.
Go to tab in your Github repository, locate the latest build and wait for it to complete.Actions
Grab the archivefirmware.zip
How to flash the keyboard?
Obtain firmware.zip
Unzip - you should have and filesfirmware.zipergonaut_one_left-seeeduino_xiao_ble-zmk.uf2ergonaut_one_right-seeeduino_xiao_ble-zmk.uf2
Turn off the power for selected halve (move slider to position OFF)
Connect selected halve to the PC via USB-C cable
Press button twice to enter DFU mode - you should see new USB device in your file managerRESET
Copy the corresponding firmware to the root directory of the new USB device
Disconnect selected halve from the PC
Repeat steps 3-7 for the other halve
How to pair halves?
Turn off the power for both halves (move slider to position OFF)
Turn on the power for both halves (move slider to position ON)
Press button once on both halves simultaneouslyRESET

---------------------05/24/2025---------------------

Adapted to zmk studio. (https://zmk.studio)

ZMK Studio provides runtime update functionality to ZMK powered devices, allowing users to change their keymap layers without flashing new firmware to their keyboards.

To learn more → https://zmk.dev/docs/features/studio.
