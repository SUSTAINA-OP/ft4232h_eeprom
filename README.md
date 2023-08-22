## Flash FT4232H EEPROM

### Setting emviroment

setting on jetson
``` sudo bash jetson_setting_lib.sh ```  
setting on linux x64
``` sudo bash x64_setting_lib.sh ```

compile code (in the firmware directory):
``` bash compile.sh ```

execute code:  
Unload Serial USB Drivers
```sudo modprobe -r ftdi_sio ```
write EEPROM ```sudo ./write```

read EEPROM data ```sudo ./read```

after write eeprom, reload Drivers:
```sudo modprobe ftdi_sio```
