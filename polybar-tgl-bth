#!/bin/sh
if [ $(bluetoothctl show | grep "Powered: yes" | wc -c) -eq 0 ]
then
  bluetoothctl power on && dunstify -a "Bluetooth" -u low Bluetooth on --icon=bluetooth-active-symbolic
else
  bluetoothctl power off && dunstify -a "Bluetooth" -u low Bluetooth off --icon=bluetooth-disconnected-symbolic
fi
