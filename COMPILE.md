# Compiling/Flashing

1. I submitted PR which contains the kintwin controller files and soft_dev keypam but it is still being reviewed. There is nothing else for me to do but wait. In the meantime, you can use the forked repo which I used for PR to flash the keyboard with new keymap

    - QMK fork url: https://github.com/alvicstep/qmk_firmware/tree/kintwin
    - kintwin controller directory url: https://github.com/alvicstep/qmk_firmware/tree/kintwin/keyboards/kinesis/kintwin
	- keymap url: https://github.com/alvicstep/qmk_firmware/tree/kintwin/keyboards/kinesis/keymaps/soft_dev
           

2. Here is a PR that I submitted for review: https://github.com/qmk/qmk_firmware/pull/21453
 
3. There is only one controller. Controller details can be found here: https://github.com/alvicstep/kintwin

4. Compiling/flashing process is the same as for any other board. QMK documentation: https://docs.qmk.fm/#/newbs_getting_started
	- download my fork of QMK (link above)
	- install QMK MSYS in order to compile the firmware: https://msys.qmk.fm  The wizard will ask whether you want to dowload QMK. Reply "no" because you already have a forked repo.
		You will then have to point MSYS to the directory where you cloned QMK fork.
		Run the following command in MSYS: `qmk config user.qmk_home=<QMK fork directory>`
		A backslash must be escaped with another backslash in the path. Example: `qmk config user.qmk_home=C:\\git\\qmk_firmware` 
		
	- compile framework. Run the following command in QMK MSYS: `qmk compile -kb kinesis/kintwin -km soft_dev`
	- download QMK Toolbox from here: https://github.com/qmk/qmk_toolbox/releases
	- put the keyboard in bootloader mode: press "Pgrogrm" button on the keyboard. This is top right button on the keyboard
	- set path in QMK Toolbox to the "bin" file which you compiled. Click "Flash" button in QMK Toolbox
	
5. To update keymap: make changes to the keymap in the forked repo here: `/keyboards/kinesis/keymaps/soft_dev/keymap.c`
   You can use any other keymap in "keymaps" directory as your base keymap. But please make sure the keymap contains bootloader mapping (code QK_BOOT). Otherwise you will have to perform physical reset by pushing buttons on the controller board itself: Hold `'boot0'` button on MCU board, press `'reset'`, then release `'boot0'`
   
   - Run the following command in QMK MSYS: `qmk compile -kb kinesis/kintwin -km <keymap name>`
   - Flash the firmware as described above
   