## oewm-project
## Outbreak Early Warning Monitor
OEWM is a web-based application that analyzes simulated non-traditional data (e.g., social media reports) 
to detect potential disease outbreaks earlier than traditional surveillance. The system calculates statistical baselines, 
triggers alerts when anomalies are detected, and visualizes alerts on a dashboard with geographical mapping.

## Features
- User Authentication (Sign Up / Login)
- Simulated data ingestion
- Running baseline calculation (14-day average)
- Anomaly detection (alerts when report spikes exceed threshold)pip install -r requirements.txt

- Alerts dashboard with historical view
- Geographic visualization of anomalies
- Time series charts showing trends

## Tech Stack
- **Frontend:** React.js
- **Backend:** Python (Flask)
- **Database:** PostgreSQL
- **Mapping API:** Mapbox or Google Maps
- **Data Processing:** Pandas, NumPy

## Installation

### Backend
1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/oewm-project.git
   cd oewm-project/backend
2. Create a virtual environment and activate it:
`bash
python3 -m venv venv
source venv/bin/activate`
3. Install dependencies
 `bash
pip install -r requirements.txt`

.4 Set up the database (PostgreSQL):
# Create database and run migration scripts 
Frontend

Navigate to frontend folder:
cd ../frontend

### Install dependencies:
npm install

Start the React development server:
npm start

---

### 6️⃣ Usage / How it Works
Explain **how to use the app**:
markdown
## Usage
1. Sign up or log in as an authorized user.
2. Navigate to the Alerts Dashboard to view current anomalies.
3. Use the map to see affected regions.
4. Check the time series charts to see trends and spikes.


7️⃣ Data Format / Seeded Data
## Seeded Data Format
The system uses a CSV file with the following columns:
- `date` (YYYY-MM-DD)
- `location_id` (ZONE_A, ZONE_B, etc.)
- `report_count` (number of reports)

Example:
date,location_id,report_count
2025-01-01,ZONE_A,12
2025-01-02,ZONE_A,15
2025-01-03,ZONE_B,8

##8️⃣ Alert Logic
- Baseline = 14-day average of report counts per location
- Standard Deviation = 14-day standard deviation
- Alert triggered if today's count > baseline + 2 * standard deviation

##9️⃣ Contributing (Optional for Teams)
## Contributing
- Create a feature branch from `main`:
  ```bash
  git checkout -b feature/branch-name



