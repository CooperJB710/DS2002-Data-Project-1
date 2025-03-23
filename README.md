## DS2002-Data-Project-1

## Project Description
This ETL pipeline retrieves vaccination data from the CDC API and population data from the U.S. Census (CSV), merges the two sources, analyzes trends by year and state, and stores the results in an SQLite database.

## Data Sources
- **CDC Vaccination API**:  
  https://data.cdc.gov/resource/8xkx-amqh.json
- **Census Population Data (CSV)**:  
  `/content/NST-EST2023-POPCHG2020_2023.csv`

## How to Use (Google Colab)
1. Upload the local CSV:  
   `NST-EST2023-POPCHG2020_2023.csv` to `/content/`
2. Run all notebook cells in order.
3. The SQLite database `etl_pipeline_database.db` will be created.
4. A download prompt will appear to save the `.db` file locally.

## Pipeline Overview
1. **Extract**  
   - CDC API data is pulled with pagination.
2. **Transform**  
   - Clean and format both datasets.
   - Merge into a unified structure.
3. **Load**  
   - Store the merged data in SQLite.
4. **Analyze**  
   - Visualize vaccinated population trends for 2021 and 2022.
   
## Authors
- Cooper Bebeau (xqt5sy)
