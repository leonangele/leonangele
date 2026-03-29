# Leon Angele

My background is in **aerospace, navigation, data fusion, and defense**, not software engineering. Code is how I realize ideas and get hands-on with the systems I'm interested in. The algorithmic design and problem framing is mine; the implementation leans heavily on AI-assisted development.

---

## Projects

### Radar Track Logging — EchoShield API Stream Reader *(private)*

I wanted to actually work with the data coming off a commercial drone-detection radar, not just observe it through a vendor interface. So I built a passive reader that decodes the raw TCP streams and writes structured output I can analyse.

**What it does:**
- Reads three simultaneous streams: confirmed tracks, raw detections, waveform parameters
- Spatially matches raw detections to confirmed tracks for per-track SNR
- Computes radial (line-of-sight) velocity from the ENU velocity vector
- Handles ECEF ↔ ENU coordinate conversion with WGS-84 georeferencing
- Pre-flight probe that checks all streams and GPS fix status before a session

`Python` `radar` `ENU/ECEF` `data fusion` `drone detection`

---

### AeroNode — Aviation Telemetry for iOS *(private)*

A tool for field navigation research and testing guided matching algorithms: an iPhone that captures synchronized video and sensor data, turning it into a precision reference instrument.

**What it does:**
- Locks a stable GNSS reference coordinate after a 60-second accuracy warm-up ("Golden Fix")
- Timestamps every video frame in UTC and links it to attitude and position data
- Fuses GPS, barometer, and IMU data into a live aviation HUD (pitch, roll, magnetic heading)
- Designed to be used cooperatively: two users with AeroNode can derive bearing to each other from their GNSS positions

`Swift` `iOS` `GNSS` `IMU fusion` `aviation` `navigation`

---

## Interests

Navigation · Applied Sensor Fusion · Guided Matching · Defense · Geospatial Data · Aerospace · Robotics
