# Project Report Draft
## Title
Patient Health Monitoring System
## Objective
Demonstrate a remote patient monitoring workflow for heart rate, body temperature and SpO₂ using an anonymized historical dataset and simulated ESP32 readings.
## Methodology
The supplied CSV is loaded with Pandas, timestamps and numeric fields are converted, and interactive visualizations are rendered using Plotly. A Python simulation produces additional readings on demand. Demonstration threshold rules generate alerts, which together with simulated measurements are stored in SQLite.
## Results
Populate this section after running the application and recording verified measurements, screenshots and test outcomes. Do not invent performance metrics.
## Limitations and future scope
The prototype has no physical sensor or MQTT broker connection. Future work includes ESP32 firmware, validated sensor integration, MQTT ingestion, calibration, secure consent-based handling, and expanded testing.
## Ethical note
Patient IDs are treated as anonymized identifiers. Do not add real patient identifiers or sensitive information. This is not a certified medical device.
