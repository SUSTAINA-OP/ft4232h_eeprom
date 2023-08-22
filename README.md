## Flash FT4232H EEPROM:

Setting emviroment:
``` sudo bash jetson_setting_lib.sh ```  

Unload Serial USB Drivers
```sudo modprobe -r ftdi_sio ```

compile code (in the firmware directory):
``` bash compile.sh ```

execute code:  
write EEPROM ```sudo ./write```

read EEPROM data ```sudo ./read```

after write eeprom, reload Drivers:
```sudo modprobe ftdi_sio```