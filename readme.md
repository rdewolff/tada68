# Tada68 keyboard

## How to program it ?

The offical way to program it is via the web site 123.57.250.164:3000/tada68 - but this web site does not work. Maybe it's just down today.

Anyway, there is a much better and easier way to program it : use the online QMK Configurator at https://config.qmk.fm. 

Steps to generate your new `FLASH.BIN` firmware :

1. Open the https://config.qmk.fm
2. Choose the keyboard `tada68`
3. Edit the keymap to suite your needs or load the one in current repo
4. Once your ready, use the `Compile` button (takes a few seconds)
5. After compilation done, you can download the firmware with the `Firemware` button.

Steps to upload your firmware on your tada68 keyboard :

1. With your keyboard plugged in, turn it's back and click the button to put in *programming* mode. It will start flashing.
2. A folder will apear on your OS, open it.
3. Backup the `FLASH.BIN` file there and replace it with your newly compiled version.
4. Once done, do not eject the drive, just hit the `Escape` key on your keyboard.
5. The keyboards stop flashing and is ready to be used!

Enjoy!

## Known issues

When deleting the old firmware and trying to copy the new one, you might have an error telling you there is not enough room on the device. This is because the OS has not cleaned the files properly. 

Solution : open the terminal and go delete the `.Trash` and `.fs-event` folder in your `/Volumes/Tada68` folder.

## References

https://config.qmk.fm
http://www.keyboardcatalog.com/65-percent/tada68#program

https://chrisabides.wordpress.com/2016/08/31/review-and-programming-tutorial-tada68/

https://www.reddit.com/r/MechanicalKeyboards/comments/50t6qi/help_tada68_programming/