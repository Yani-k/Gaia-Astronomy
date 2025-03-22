# Gaia-Astronomy
# High Parallax Star Analysis

## Overview
This project, completed as part of the *Programming for Analytics* course at Baruch College, analyzes high-parallax stars using Gaia DR3 data. The script queries nearby stars, classifies them based on temperature, and visualizes key stellar properties.

## Features
- Queries Gaia DR3 data for high-parallax stars (stars relatively close to Earth)
- Converts parallax measurements into light years
- Classifies stars based on temperature
- Provides statistical summaries and visualizations
- Saves results to a CSV file and an SQLite database

## Requirements
To run this project, install the following dependencies:
```sh
pip install astroquery pandas seaborn matplotlib sqlite3
```

## Usage
1. **Run the script** to fetch Gaia DR3 data and process it:
   ```sh
   python star_analysis.py
   ```
2. **Output:**
   - A CSV file: `high_parallax_stars.csv`
   - An SQLite database: `star_data.db`
   - Various visualizations including histograms and scatter plots

## Key Functions
- `query_nearby_star_data()`: Retrieves data from Gaia DR3
- `convert_parallax_to_lightyears()`: Converts parallax to distance
- `get_stellar_class()`: Classifies stars based on temperature
- `print_summary()`: Prints dataset statistics
- `visualize_data()`: Generates visualizations
- `save_results_to_csv()`: Saves data to CSV
- `save_results_to_db()`: Stores data in SQLite

## Example Output
- **Total Stars Retrieved:** 1160
- **Temperature Range:** 2809K - 7938K
- **Stellar Class Distribution:**
  - A: 1
  - F: 47
  - G: 102
  - K: 206
  - M: 804

## License
This project is for educational purposes as part of the Baruch College *Programming for Analytics* course.

## Author
[Your Name]

