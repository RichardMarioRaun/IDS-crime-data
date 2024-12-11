# Project C12 - Crime Rates in LA, Chicago, and Portland Compared to Vancouver

## Team Members

**Andreas Kelder, Richard Mario Raun**

### Motivation and Goal

Crime rates are a significant indicator of urban safety, and the comparison between U.S. cities and a Canadian city provides fascinating insights into cultural, policy, and enforcement differences. This project aimed to uncover how crime rates in Vancouver stack up against three major U.S. cities—Los Angeles, Chicago, and Portland—to identify patterns and trends that inform public safety and urban planning.

### Guide to Repository Contents

1. **README.md:** This file provides an overview of the project, methods, results, and insights.
2. **data/**: Contains raw data the place where datasets should be downloaded.
3. **DataWorkbook.ipynb**: Jupyter notebook documenting the data preparation, analysis, and visualization steps.
4. **scripts/**: Python script for data processing.
5. **IDS-Raun-Kelder.pdf**: Poster for presentation.

### Replicating the Analysis

To replicate the analysis:

1. Clone this repository: `git clone https://github.com/RichardMarioRaun/IDS-crime-data`
2. Download the datasets and rename them in the following format(city_crime.csv)
3. Install the required Python dependencies.
4. Run the Jupyter notebooks sequentially to reproduce the results.

## Introduction

Everyone loves true crime stories, and many of them originate from the U.S., a country with a notably high prison population. But how do crime rates in U.S. cities compare to their neighbor to the north, Canada? This project investigates crime rates, severity, and patterns across four cities—Los Angeles, Chicago, Portland, and Vancouver—to determine the differences in urban safety.

## Overview of Results

1. Vancouver boasts the lowest crime rates among the four cities, with crimes there being less severe on average—primarily burglaries.
2. Chicago is the most dangerous, with approximately 614 crimes committed daily, with theft being the most common.
3. All cities show a decline in crime rates over time, with crime spikes around midday.

## Methods and Tools

### **Data Sources**

- Crime data from Kaggle, including datasets for Vancouver, Portland, Los Angeles, and Chicago.
- Population statistics sourced from google.

### **Tools Used**

- **Python Libraries:** pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Folium, Geopandas, Plotly, Pyproj and Shapely.
- **Visualization:** Matplotlib, Canva.
- **Development Environment:** Jupyter Notebook.

### **Analysis Steps**

1. **Data Cleaning and Preprocessing:** Standardized formats across datasets, including timestamps and crime categories.
2. **Geospatial Analysis:** Mapped crime hotspots and calculated density.
3. **Crime Severity Index Development:** Weighted crimes by severity to compare their impact meaningfully.
4. **Temporal Analysis:** Identified patterns based on time of day and season.
5. **Visualization:** Used heatmaps, bar graphs, and line charts to illustrate findings effectively.

## Project Plan and Tasks

### Initial project plan

1. **Data Collection and Preparation (12 hours total):**  
   - **Hours per Member:** Andreas (6 hours), Richard (6 hours)  
   - **Description:** Collect datasets, verify availability, and preprocess data (cleaning, integration, normalization). This includes standardizing crime categories and converting timestamps.  
   - **Tools/Methods:** Python (pandas, NumPy), Jupyter Notebook.  
2. **Exploratory Data Analysis (EDA) (10 hours total):**  
   - **Hours per Member:** Andreas (5 hours), Richard (5 hours)  
   - **Description:** Perform initial data exploration, analyze distributions, and identify trends. Generate visualizations for seasonal and time-of-day patterns.  
   - **Tools/Methods:** Matplotlib, Seaborn, descriptive statistics in Python.  
3. **Crime Severity Index Development (8 hours total):**  
   - **Hours per Member:** Andreas (4 hours), Richard (4 hours)  
   - **Description:** Create a weighted severity index for crime types and compute indices for each city. Validate and interpret results.  
   - **Tools/Methods:** Python (custom weighting functions).  
4. **Modeling and Pattern Analysis (14 hours total):**  
   - **Hours per Member:** Andreas (7 hours), Richard (7 hours)  
   - **Description:** Use machine learning models to analyze crime trends and predict seasonal or temporal patterns.  
   - **Tools/Methods:** scikit-learn for regression models, Python for data transformations.  
5. **Visualization and Reporting (16 hours total):**  
   - **Hours per Member:** Andreas (8 hours), Richard (8 hours)  
   - **Description:** Develop visualizations to communicate findings clearly and compile the final report. Prepare a presentation and poster for the project showcase.  
   - **Tools/Methods:** Matplotlib, Canva (for poster), Google Docs for report writing.

## Key Insights and Visualizations

1. **Overall Crime Rates:**
   - Vancouver had a lower crime rate than LA and Chicago but was comparable to Portland.
2. **Crime Severity:**
   - Violent crimes were most prevalent in LA, while Vancouver had higher rates of property crimes.
3. **Temporal Patterns:**
   - Crime rates spiked during summer evenings in all cities, with noticeable dips during early morning hours.

## Challenges and Mitigations

1. **Inconsistent Data Categories:** Resolved by mapping categories to a unified schema.
2. **Coordinates formating:** Resolved by converting all coordinates to the same format/measuring system.
3. **Missing Coordinates:** Resloved by making 2 differnet datasets. One for heatmaps(drops all invalid coordinates) and one for pure crime data(doesnt drop invalid coordinates)

## Conclusion and Recommendations

This analysis provided actionable insights into crime trends and relative safety across cities. Based on the findings:

- Vancouver is a safer travel destination compared to LA and Chicago.
- Community policing and resource allocation should focus on evening hours during summer months to mitigate crime spikes.

## Acknowledgments

Special thanks to Kaggle for providing the datasets and to our academic advisors for their guidance throughout this project.

---
**Data Sources:**

- [Los Angeles Crime Data](https://www.kaggle.com/datasets/middlehigh/los-angeles-crime-data-from-2000?select=Chicage+Crime+Data.csv)  
- [Portland Crime Data](https://www.kaggle.com/datasets/michaellindsay/portland-crime)  
- [Vancouver Crime Data](https://www.kaggle.com/datasets/tcashion/vancouver-bc-crime-dataset?select=crimedata_csv_AllNeighbourhoods_AllYears.csv)  
- [Chicago Crime Data](https://www.kaggle.com/datasets/adelanseur/crimes-2001-to-present-chicago?resource=download)
