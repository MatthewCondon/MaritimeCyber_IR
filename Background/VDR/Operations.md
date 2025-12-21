# Voyage Data Recorder
Similar to aircraft storing all flight logs and data in a black box recorder, vessels have been outfitted with a Voyage Data Recorder (VDR) for the same purpose. The VDR is mandated by the International Maritime Organization through Safety of Life at Sea (SOLAS) regulations. Acting as an additional node on the NMEA 2000 backbone, the VDR is responsible for monitoring and recording all information exchanged between vessel devices on the data bus. Information tracked by the VDR include, but is not limited to, Global Positioning System (GPS), radar and contacts, depth readings, speed logs, engine and fuel status, and wind measurements. By tracking the sources of data, the VDR can be used during investigations in the event of a maritime incident. Operating as a cohesive protocol, this piece of equipment ensures data is available for investigators post-incident. The solid-state memory ensures that the capsule has, at a minimum, recordings of at least the last 12 to 24 hours and can withstand environmental damage.

There are various kinds of Voyage Data Recorders. Common variations are pictured below:

<table>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/d03918ca-a801-491b-9b25-51611b1aaae2" width="500"/></td>
    <td><img src="https://github.com/user-attachments/assets/02951109-45ff-4d6b-8066-e3998e3c4172" width="500"/></td>
  </tr>
</table>

The Voyage Data Recorder uses proprietary software to organize collected NMEA data into precise time-based groupings. This system ensures that navigational, sensor, and communication information are synchronized accurately, allowing investigators to reconstruct events in chronological order and analyze vessel performance, communications, and incidents with high accuracy.

# National Transportation Security Board (NTSB)
The NTSB is responsible for posting previously collected and analyzed data from maritime incidents. The link for their website can be accessed at: https://www.ntsb.gov/Pages/home.aspx

Depending on what is searched, most of the results will provide a PDF with findings and overall results from the incident. Searching "VDR CSV" will yield results with real VDR data to download and analyze. 

While not directly related to the scope of forensic analysis, this is a good starting point to determine what good data may look like before an apparent incident.
