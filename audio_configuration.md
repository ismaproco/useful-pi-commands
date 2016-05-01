# Commands to configure the audio in raspberry pi

Reason
-------

Some times the raspberry pi audio output changes from the analog to the hdmi, or this change can also be performe by desire.

The internal codes for the outputs are:

* Auto: 0
* Analog: 1
* HDMI: 2

- Use the amixer.

``` 
amixer cset numid=3 2
```

- Use the raspberry config file.

``` 
sudo raspi-config
```

- Update the config file.

```
sudo vim /boot/config.txt 
```

set variable 
```
hdmi_drive=2
```

and reboot
