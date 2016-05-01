# Reproduce music in Raspberry pi from mp3 or spotify

- Commands to manage the music service
```
# start the service
sudo systemctl start mopidy

# add the service to the system
sudo systemctl enable mopidy

# check the status of the service
sudo systemctl status mopidy
```

- to edit the configuration of the application

```
# if running as a service
sudo vim /etc/mopidy/mopidy.conf

# if running as app
vim ~/.config/mopidy/mopidy.conf
```

The application start a webserver to manage the application in port: `6680`, and the application itself run in port `6600`
