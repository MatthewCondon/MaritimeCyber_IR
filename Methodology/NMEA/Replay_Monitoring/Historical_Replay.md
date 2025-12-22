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

# Ensuring Interface Status
Once the interface has been set, it is important to ensure it is ```UP``` and ready to process data with the Raspberry Pi.
```
ip -details link show can0
```
_This command has output. The relevant detail is:_
```
4: can0: <NOARP,UP,LOWER_UP,ECHO> mtu 16 qdisc pfifo_fast state UP mode DEFAULT group default qlen 10
```

# Sending NMEA Frames
After the data is converted into the Raw SocketCAN format, place it into a file. Using ```canplayer```, send the data file onto the NMEA backbone.
```
canplayer -I file.log -t
```
_This command has no output associated with it. To stop running the command, use ```Ctrl + C```._

The boat should begin replaying data at this time. All display systems will show the relevant information from the data file.

# Replay Analysis
When running data through the NMEA backbone, watch the displays for any abnormal behavior. Compare the information shown on different displays, such as equipment displays directly connected to machinery to monitors on the bridge.
