# Data Collection
A Voyage Data Recorder (VDR) is a shipboard system designed to continuously collect, synchronize, and store operational and navigational data from across a vessel. It passively receives information from multiple onboard sensors and systems using standard marine data interfaces, such as NMEA 0183 and NMEA 2000. Common inputs include GPS position and time, vessel speed and heading, radar imagery and target data, depth measurements, bridge audio (including internal microphones and VHF radio traffic), alarms, and selected machinery and engine parameters.

# Data Processing
The VDR processes these inputs by time-stamping and organizing them into a continuous recording, typically maintained in a rolling buffer that preserves at least the most recent 48 hours of data. As new information is recorded, older data is overwritten unless an incident causes the data to be retained for investigation. To ensure survivability, the final recording medium is housed in a hardened, tamper-resistant capsule capable of withstanding extreme conditions such as fire, flooding, impact, and high pressure.

# Data Example
Much of the information that may be collected from the VDR includes radio communication and bridge audio recordings, radar contacts images, and ship coordinate maps. An example of extracted VDR data is pictured below:
<img width="550" height="162" alt="image" src="https://github.com/user-attachments/assets/528f233f-a615-4344-8c4a-282319d3331b" />
