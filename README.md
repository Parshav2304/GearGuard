# 🔧 GearGuard - Asset Maintenance & Equipment Tracker

**GearGuard** is a feature-rich, interactive asset maintenance tracker designed for engineering teams, workshops, and facilities. Built entirely on **Streamlit** with custom CSS styling, GearGuard implements a complete work-order management flow, calendar-based scheduling, equipment databases, and analytical performance metrics to minimize asset downtime.

---

## 🎨 Application Architecture

```
                       ┌────────────────────────┐
                       │  Streamlit App Engine  │
                       │       (app.py)         │
                       └───────────┬────────────┘
                                   │
         ┌──────────────┬──────────┼──────────────┬──────────────┐
         ▼              ▼          ▼              ▼              ▼
   [ Kanban Board]  [ Calendar] [Equipment]   [ Teams ]     [ Analytics ]
     kanban.py      calendar_   equipment.py   teams.py     analytics.py
                      view
```

---

## ✨ Features & Modules

- **🎯 Kanban Board (`kanban.py`)**: A visual, interactive board to manage maintenance request states (`New`, `In Progress`, `Resolved`). Move work orders across columns, track priority metrics, and assign tasks to teams.
- **📅 Maintenance Calendar (`calendar_view.py`)**: Schedules and coordinates inspections, calibrations, and preventive maintenance periods to avoid critical equipment failures.
- **⚙️ Equipment Catalog (`equipment.py`)**: Stores and manages detailed hardware asset sheets, including manufacturer information, warranty limits, purchase history, and maintenance schedules.
- **👥 Team Allocations (`teams.py`)**: Manages technical staff assignments, logs working schedules, and correlates tasks to teams.
- **📊 Performance Analytics (`analytics.py`)**: Renders visual summaries of equipment health, MTTR (Mean Time to Repair), cost distributions, and frequency of breakdowns.

---

## 🛠️ Tech Stack

- **Python 3.9+**
- **Streamlit** - Core UI and dashboard framework.
- **Pandas** - Telemetry and asset spreadsheet processing.
- **Matplotlib / Seaborn** - Analytical charts and metric tracking.
- **Custom CSS** - Dynamic frosted-glass gradient dashboard styling.

---

## 🚀 Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/Parshav2304/GearGuard.git
cd GearGuard
```

### 2. Install Dependencies
Create a virtual environment and install the requirements:
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

pip install -r requirements.txt
```

### 3. Run the Dashboard
Start the Streamlit application:
```bash
streamlit run app.py
```
*(The dashboard will open automatically on `http://localhost:8501`)*

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.
