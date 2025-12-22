# Overview
When collecting data, it will be in the **Compact Human-Readable** format.
```
  can0  09F11240   [8]  FF 69 00 FF 7F FF 7F FC
```

# Setting the Interface
A connection to the interfaceis necessary to collect live data. 
Create the interface and set the necessary bit rate for NMEA 2000 networks. The restart occurs in the event an off-string is sent the network needs to be restarted.
```
sudo ip link set can0 up type can bitrate 250000 restart-ms 100
```
_This command has no output associated with it._

# Collecting Data Frames
To collect data, the use ```candump``` with the previously created interface. Save this output to a file.
```
candump can0 > file.log
```
This command has no output associated with it. To stop running the command, use Ctrl + C.

# Monitoring Analysis
When collecting live data, look for abnormal behavior by devices, such as certain frames being repeated too many times on the interface when compared to others.

Most equipment on the vessel should still be operational. By connecting to the live NMEA backbone, it is important to determine if any equipment is not sending any frames or sending incorrect frames. This may indicate equipment that has malfunctioned and requires closer inspection.
