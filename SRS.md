# Software Requirements Specification
## Purpose
Build an academic patient health monitoring dashboard using supplied CSV records and a simulated ESP32 data source.
## Functional requirements
1. Load and validate the supplied dataset.
2. Show patient-level and overall vital statistics.
3. Visualize heart rate, body temperature and SpO₂ trends.
4. Generate simulated readings on demand.
5. Apply configurable demonstration thresholds and store generated alerts.
6. Store simulated measurements and alerts in SQLite.
7. Filter patient records and export CSV/Excel.
## Non-functional requirements
Readable modular code, local execution, no hardcoded credentials, preserve source data, clear simulation labels, and responsive dashboard layout.
## Constraints
No physical ESP32 or sensors are assumed; MQTT is not connected in this rapid prototype. The system is not for clinical use.
