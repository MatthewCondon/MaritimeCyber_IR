# Overview
To replay historical data, it must be in the **Raw SocketCAN** format.

```
(1759512073.077585) can0 09F20540#00FCAC0D1B0E00FF
```

# Setting Replay Interface
A connection to the ```can0``` interface must be established before data can be sent.
```
sudo ip link set can0 up type can bitrate 250000 restart-ms 100
```
_This command has no output associated with it._


After configuring the interface in the Raspberry Pi, the ```can0``` interface must be set to replay and send data back into the NMEA backbone.
```
sudo ip link set can0 txqueuelen 10000
```
_This command has no output associated with it._

# Sending NMEA Frames
After the data is converted into the Raw SocketCAN format, place it into a file. Using ```canplayer```, send the data file onto the NMEA backbone.
```
canplayer -I file.log -t
```
_This command has no output associated with it. To stop running the command, use ```Ctrl + C```._

The boat should begin replaying data at this time. All display systems will show the relevant information from the data file.
