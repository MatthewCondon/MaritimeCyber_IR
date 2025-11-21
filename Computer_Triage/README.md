# Importance of Triage
Modern vessels depend on complex digital ecosystems—navigation suites, engineering control systems, communication networks, and administrative computers—all of which can generate critical evidence during a maritime incident. As a result, computer triage and analysis of electronic equipment has become a central component of maritime investigations, supporting accurate reconstruction, root-cause identification, and regulatory or legal conclusions.

A helpful way to visualize the investigative workflow is captured in the following cycle:

<p align="center">
  <img src="https://github.com/user-attachments/assets/c80343b0-a944-4eb0-9a12-74c2e14f4b66" width="400" height="354" />
</p>

Beyond identifying evidence, triage guides the forensic strategy. Many maritime networks contain a mix of IT and OT systems, each with different risks and acquisition methods. A live ICS system controlling propulsion or steering cannot simply be imaged like a standard PC; investigators must evaluate the safety implications of pulling power or interfacing with controllers. Likewise, NMEA-2000 and CAN-bus devices often store data in volatile memory or proprietary buffer formats, requiring immediate capture using specialized gateways or direct bus sniffing. Early triage helps ensure the right tools—packet capture devices, write blockers, CAN-bus loggers, forensic imaging suites—are deployed appropriately.

Computer analysis also provides critical context during reconstruction of the incident. For example, correlating VDR audio with network logs, radar tracks, and engine-room control messages can reveal timing discrepancies, mechanical failures, incorrect inputs, spoofed navigation data, or signs of cyber manipulation. Deep analysis of PCs and servers may uncover email communications, malware activity, unauthorized remote access, or misconfigurations that contributed to the event. In regulatory or legal contexts, such findings support accurate attribution and improve safety recommendations.
