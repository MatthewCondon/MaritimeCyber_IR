# PGN Reference Table

### Key:
- 🟥 **High Priority**
- 🟨 **Medium Priority**
- 🟩 **Low Priority**

---

## Core / ISO PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟩 | 59392 | ISO Acknowledgement | - | |
| 🟩 | 59904 | ISO Request | - | |
| 🟩 | 60160 | ISO TP: Data Transfer | - | |
| 🟩 | 60416 | ISO TP: Connection Management | - | |
| 🟩 | 60928 | ISO Address Claim | - | |
| 🟩 | 65240 | Commanded Address | - | |

---

## System PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟨 | 126208 | NMEA Group Function | - | |
| 🟨 | 126464 | PGN List | - | |
| 🟨 | 126996 | Product Information | - | |
| 🟨 | 126998 | Configuration Information | - | |
| 🟥 | 126992 | System Time | Seconds | |

---

## Steering / Motion PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟥 | 127237 | Heading/Track Control | Degrees | |
| 🟥 | 127245 | Rudder | Degrees | |
| 🟥 | 127250 | Vessel Heading | Degrees | |
| 🟥 | 127251 | Rate of Turn | Degrees/MIN | |
| 🟨 | 127252 | Heave | Degrees | |
| 🟥 | 127258 | Magnetic Variation | Degrees/MIN | |

---

## Engine / Mechanical PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟥 | 127488 | Engine Parameters, Rapid Update | RPM | |
| 🟨 | 127489 | Engine Parameters, Dynamic | Degrees C / kPA / Volts / Percent | |
| 🟥 | 127493 | Transmission Parameters | RPM / Degrees C / kPA / Gear State | |
| 🟨 | 127497 | Trip Parameters, Engine | Liters / Hours / kWh / Percent | |
| 🟩 | 127501 | Binary Switch Bank Status | On/Off | |
| 🟩 | 127502 | Switch Bank Control | On/Off | |
| 🟨 | 127503 | AC Input Status | Volts / Amps / Hertz | |
| 🟨 | 127504 | AC Output Status | Volts / Amps / Hertz | |
| 🟩 | 127505 | Fluid Level | Percent | |
| 🟨 | 127506 | DC Detailed Status | Volts / Amps / State | |
| 🟨 | 127507 | Charger Status | Volts / Amps / Percent | |
| 🟨 | 127508 | Battery Status | Volts / Amps / Temperatures | |
| 🟨 | 127509 | Inverter Status | Volts / Amps / Hertz | |
| 🟨 | 127510 | Charger Configuration | Volts / Amps / Percent | |

---

## Navigation PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟥 | 129025 | Position, Rapid Update | Degrees | |
| 🟥 | 129026 | COG & SOG | Degrees and Knots | |
| 🟥 | 129027 | Position Delta | Latitude Delta / Longitude Delta | |
| 🟥 | 129028 | Altitude Delta | Meters | |
| 🟥 | 129029 | GNSS Position Data | Days / Seconds / Degrees / Degrees / Meters | |
| 🟨 | 129033 | Local Time Offset | Hours and Minutes | |
| 🟨 | 129044 | Datum | Degrees and Knots | |
| 🟨 | 129045 | User Datum Settings | Degrees / Meters | |
| 🟥 | 129283 | Cross Track Error | Yards | |
| 🟥 | 129284 | Navigation Data | meters / seconds / days / radians / meter per second | |
| 🟨 | 129285 | Route/WP Info | meters | |
| 🟨 | 129291 | Set & Drift | meters | |
| 🟨 | 129301 | Time to/from Mark | Hours / Minutes / Seconds | |

---

## AIS PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟥 | 129038 | AIS Class A Position | Degrees / Knots / Seconds | |
| 🟥 | 129039 | AIS Class B Position | Degrees / Knots / Seconds | |
| 🟨 | 129040 | AIS Class B Extended | Degrees / Knots / Seconds / Meters | |
| 🟨 | 129041 | AIS AtoN Report | Degrees / Meters / Seconds | |
| 🟨 | 129793 | AIS UTC & Date | Hours / Minutes / Seconds / Days | |
| 🟨 | 129794 | AIS Class A Static/Voyage Data | Mixed Fields | |
| 🟥 | 129795 | AIS Aircraft Position | Degrees / Knots / Seconds | |
| 🟨 | 129797 | AIS Binary Broadcast | Binary Data | |
| 🟨 | 129798 | AIS SAR Aircraft | Degrees / Knots / Seconds | |
| 🟨 | 129799 | AIS Safety Related | Text | |
| 🟨 | 129802 | AIS Addressed Safety Message | Text | |
| 🟨 | 129809 | AIS Class B Static Data Part A | Alphanumeric | |
| 🟨 | 129810 | AIS Class B Static Data Part B | Alphanumeric | |

---

## GNSS / Satellite PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟨 | 129539 | GNSS DOPs | Dimensionless | |
| 🟩 | 129540 | GNSS Sats in View | Count | |
| 🟩 | 129541 | GNSS Almanac | Orbital Parameters | |
| 🟩 | 129542 | GNSS Ephemeris | High-precision Orbital Data | |

---

## Route & Waypoint PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟩 | 130066 | Route/WP List Attributes | - | |
| 🟩 | 130067 | Route — WP Name & Position | Degrees / Meters | |
| 🟩 | 130068 | WP Group List | - | |
| 🟩 | 130074 | WP List — WP Name & Position | Degrees / Meters | |

---

## Environmental / Weather PGNs

| Priority | PGN | Name | Data Type | Detecting Anomalies |
|----------|-----|-------|-----------|----------------------|
| 🟥 | 130306 | Wind Data | Knots / Degrees | |
| 🟨 | 130310 | Environmental Parameters | Degrees C / kPA / %RH | |
| 🟨 | 130311 | Environmental Parameters | Degrees C / kPA / %RH | |
| 🟨 | 130312 | Temperature | Degrees C | |
| 🟨 | 130313 | Humidity | Percent | |
| 🟨 | 130314 | Actual Pressure | kPA | |
| 🟨 | 130316 | Extended Temperature | Degrees C | |
| 🟥 | 130320 | Sea Temperature | Degrees C | |
| 🟨 | 130321 | Salinity | PSU | |
| 🟨 | 130322 | Tide Station Data | Meters | |
| 🟨 | 130323 | Meteorological Station Data | Mixed | |
| 🟨 | 130324 | Weather Report | Mixed | |
| 🟨 | 130577 | Direction Data | Degrees | |
