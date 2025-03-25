# Cheap Yellow Display on Tasmota

## Tasmota firmware

Install OTA firmware 13.4.0 from http://ota.tasmota.com/tasmota32/release-13.4.0/tasmota32-lvgl.bin

## Set the template

In the menu `Configuration -> Configure Other -> Template`

Set the value to the json from `template.json`

## Upload files

In `Tools -> Manage File system`

Upload `display.ini` and `autoexec.be`

display.ini from https://templates.blakadder.com/sunton_ESP32-2432S028.html but resolution line swapped 

autoexec.be from https://templates.blakadder.com/sunton_ESP32-2432S028.html but event.code swapped for event.get_code()

## Calibrate screen

From https://tasmota.github.io/docs/Tasmota-Application/#display-calibration

In `Tools -> Manage File system`

Upload DisplayCalibrate.tapp

Restart

In `Tools -> Console`

Enter the command `DisplayCalibrate`

Then follow the instructions on the display
