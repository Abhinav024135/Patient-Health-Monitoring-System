# Patient Health Monitoring System

**HCLTech Career Shaper Programme | Project 4 | Embedded IoT**

A Streamlit academic prototype for exploring patient vital-sign records and demonstrating a simulated ESP32 monitoring workflow.

## Features
- Dashboard KPIs and interactive Plotly charts
- Patient-wise historical records and trends
- Python-generated simulated ESP32 readings
- Configurable demonstration threshold alert engine
- SQLite persistence for simulated readings and alerts
- Dataset quality explorer and cleaned CSV export
- CSV and Excel report export
- Data dictionary descriptions

## Dataset
The supplied `data/dataset.csv` is preserved without changing its original column names:
`timestamp`, `patient_id`, `heart_rate_bpm`, `body_temp_C`, `SpO2_pct`, `comm_channel`, `alert_flag`.

## Run on Windows PowerShell
```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
streamlit run app.py
```

## Architecture
Historical CSV / simulated ESP32 readings -> Python data and alert logic -> SQLite -> Streamlit UI and Plotly charts.

MQTT and physical ESP32 integration are future integration points; this prototype does not claim to connect to physical sensors or a broker.

## Important limitations
- Academic demonstration only; not a certified medical device.
- Simulated readings are clearly labelled and must not be represented as physical measurements.
- Thresholds are illustrative software rules, not universal clinical diagnostic standards.
- No real patient names or personally identifiable information are collected.
- The app provides CSV and Excel exports. PDF report generation is deferred in this rapid prototype.

## AI use disclosure
Disclose any AI-assisted code generation or writing according to programme requirements and verify all generated material before submission.
