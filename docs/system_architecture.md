# System Architecture
```text
Supplied dataset.csv -----------+
                                +--> Python/Pandas data layer --> Streamlit dashboard
Simulated ESP32 readings -------+                 |                    |
                                                  +--> Alert rules      +--> Plotly charts
                                                  |                    +--> CSV/Excel export
                                                  +--> SQLite database

Future extension: Physical sensors -> ESP32 -> Wi-Fi/MQTT -> ingestion service -> SQLite/dashboard
```
## Level 0 data flow
External data sources (historical CSV and simulated ESP32) provide anonymized vital readings. The monitoring application validates and processes readings, stores simulation records and alerts, and presents charts, tables and downloadable reports to the learner.
