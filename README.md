# California Crash Analysis (EDA)

Exploratory data analysis of California’s 2025 YTD (Jan-Aug) crash dataset from the California Crash Reporting System (CCRS), using Python (pandas, numpy, plotly).

## Objective

Analyze how collision types and involved parties impact:
- **Frequency** (how often crashes occur)
- **Severity** (injuries per crash)

**Data Source:** California Crash Reporting System (CCRS)  
https://data.ca.gov/dataset/ccrs  

---

## Key Insights

- Pedestrian crashes are disproportionately severe relative to frequency  
- Broadside collisions combine **high frequency and high severity**  
- Rear-end collisions are **most common but less severe**  
- Bicycle crashes show elevated injury severity compared to vehicle-only incidents  

---

## Methodology

- Cleaned and standardized raw CCRS dataset  
- Removed columns with >70% missing values  
- Validated `Collision_id` as a unique identifier  
- Compared frequency and severity across:
  - Involved party type  
  - Collision type  
- Visualized patterns using bar charts and frequency vs. severity scatter plots  

---

## Visualizations

### Involved Party

- **Frequency** – Other motor vehicles dominate crash counts  
![Involved Party Frequency](figures/involved_party_frequency.png)

- **Severity** – Pedestrian and bicycle crashes have the highest injuries  
![Involved Party Severity](figures/involved_party_severity.png)

- **Frequency vs Severity** – Pedestrian crashes combine high severity with meaningful frequency  
![Involved Party Scatter](figures/involved_party_scatter.png)

---

### Collision Type

- **Frequency** – Rear-end collisions are most common  
![Collision Type Frequency](figures/collision_type_frequency.png)

- **Severity** – Pedestrian, broadside, and head-on collisions are most dangerous  
![Collision Type Severity](figures/collision_type_severity.png)

- **Frequency vs Severity** – Broadsides stand out as both frequent and severe  
![Collision Type Scatter](figures/collision_type_scatter.png)

---

## How to Run

1. Install dependencies  
   `pip install -r requirements.txt`  

2. Download dataset and save as  
   `crashes_dataset.csv`  

3. Run the notebook  
