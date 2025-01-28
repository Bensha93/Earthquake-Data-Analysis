# 🌍 Earthquake Data Analysis: A Comprehensive Statistical Investigation of Global Seismic Events

## **📊 Project Overview**
This analysis explores global seismic activity using data from the USGS (United States Geological Survey) Earthquake Catalog. Through comprehensive data wrangling, statistical analysis, and visualization techniques, this project uncovers patterns and relationships in earthquake occurrences worldwide.

---

## **🎯 Objectives**
- Investigate the spatial and temporal distribution of earthquakes.
- Analyze relationships between earthquake characteristics (magnitude, depth, location).
- Identify potential patterns in seismic activity.
- Assess regional variations in earthquake occurrences.
- Develop statistical insights into global seismic patterns.

---

## **📑 Dataset Description**
The dataset contains detailed information about earthquakes, including:
- **Event location**: Longitude and latitude.
- **Magnitude and depth**: Measurement details of seismic activity.
- **Temporal information**: Date and time of events.
- **Additional seismic measurements**: Various indicators of activity.
- **Regional metadata**: Details about the region of occurrence.

---

## **🔍 Methodological Approach**
### **1️⃣ Data Preprocessing and Wrangling**
- Cleaning and structuring raw seismic data.
- Handling missing values.
- Creating derived features for enhanced analysis.
- Standardizing measurements across observations.

### **2️⃣ Statistical Analysis**
- Descriptive statistics of earthquake characteristics.
- Hypothesis testing for regional differences.
- Correlation analysis between seismic parameters.
- Bootstrap sampling for robust statistical inference.

### **3️⃣ Visual Analytics**
- Geographic distribution mapping.
- Temporal trend visualization.
- Relationship plots between key variables.
- Interactive dashboards for exploration.

### **4️⃣ Insight Generation**
- Pattern identification in seismic activity.
- Regional risk assessment.
- Temporal trend analysis.
- Correlation discovery between variables.

---

## **💻 Technical Implementation**
This analysis uses **R programming language** with the following key libraries:
- `dplyr` for data manipulation.
- `ggplot2` for visualization.
- `tidyr` for data cleaning.
- `stats` for statistical analysis.

---

## **🎁 Expected Outcomes**
- Clear understanding of global earthquake patterns.
- Statistical validation of seismic relationships.
- Visual representation of complex earthquake data.
- Actionable insights for seismic risk assessment.

---

## **🚀 Data Processing Workflow**
### **Initial Data Collection and Processing**
- **Source**: USGS Earthquake Catalog API.
- **Period**: Earthquakes recorded from **November 8, 2024**, to **December 20, 2024**.
- **Steps**:
  1. Imported essential R libraries (`jsonlite`, `tidyr`, `dplyr`).
  2. Collected raw data in JSON format and transformed it into a comprehensive dataframe.
  3. Flattened nested JSON structures for easier analysis.

### **Key Features of Processed Data**
- **Geographic coordinates**: Longitude, latitude, and depth.
- **Temporal details**: Converted Unix timestamps to human-readable dates.
- **Location metadata**: Standardized city, state, and country details.
- **Numeric imputation**: Mean imputation for missing seismic metrics.
- **Derived columns**: Added columns for earthquake age and geographic classifications.

---

## **🌟 Data Cleaning and Transformation**
### **1. Coordinate Extraction**
- Extracted longitude, latitude, and depth from nested JSON fields.

### **2. Time Standardization**
- Converted Unix timestamps into readable datetime formats for better temporal analysis.

### **3. Location Processing**
- Standardized city and state information.
- Added a **country** column with logic to handle special cases (e.g., oceanic regions assigned to "International Waters").

### **4. Missing Data Treatment**
- Handled missing values with mean imputation for numeric fields such as:
  - Number of seismic stations.
  - Minimum distance to seismic stations.
  - Azimuthal gap.

### **5. Geographic Classification**
- Categorized earthquakes by continent based on geographic coordinates.

---

## **📊 Data Categorization and Classification**
### **Magnitude Classification**
- Minor: Magnitude < 2.0.
- Light: 2.0 ≤ Magnitude < 4.0.
- Moderate: 4.0 ≤ Magnitude < 6.0.
- Major: Magnitude ≥ 6.0.

### **Depth Classification**
- Shallow: Depth < 70 km.
- Intermediate: 70 km ≤ Depth < 300 km.
- Deep: Depth ≥ 300 km.

---

## **📈 Statistical Analysis Results**
### **ANOVA: Relationship Between Magnitude and Depth**
- **Degrees of Freedom**:
  - Magnitude Category: 3.
  - Residuals: 15,641.
- **Sum of Squares**:
  - Between groups: 7,963,588.
  - Within groups: 37,284,463.
- **F-Value**: 1,114 (high, indicating significant group differences).
- **P-Value**: < 2e-16 (extremely significant).

---

## **🎨 Visual Analysis**
### **1. Geographic Distribution**
- Scatter plot highlighting earthquake concentrations along tectonic plate boundaries:
  - Pacific Ring of Fire.
  - Mid-Atlantic Ridge.

### **2. Magnitude by Depth Categories**
- **Deep Earthquakes**: Consistent magnitude patterns (peak: 4.5–5.0).
- **Intermediate Earthquakes**: Bimodal distribution.
- **Shallow Earthquakes**: Normal distribution with variable ranges.

---

## **📊 Bootstrap Analysis**
### **Bootstrap Distribution of Mean Magnitude**
- **Mean Magnitude**: 1.64.
- **95% Confidence Interval**: 1.62–1.66.
- **Key Insights**:
  - Narrow confidence interval indicates high precision.
  - Reliable framework for earthquake magnitude predictions.

---

## **⏳ Temporal Analysis**
### **Hourly Frequency Patterns**
- **Peak Activity**: 9:00 AM UTC (~615 earthquakes).
- **Secondary Peaks**: Midnight UTC, 5:00 AM, and 8:00 PM.
- **Cyclical Trends**: ~4–6 hour cycles between activity peaks.

---

## **🛠️ Technical Skills**
- **Data Collection**:
  - USGS Earthquake API integration.
  - JSON data handling.
- **Programming**:
  - R programming (dplyr, ggplot2, tidyr, lubridate).
- **Statistical Analysis**:
  - ANOVA, correlation, and bootstrap sampling.
- **Visualization**:
  - Geographic mapping and temporal trend analysis.

---

## **📊 Future Directions**
- Implement real-time monitoring.
- Develop predictive models for seismic activity.
- Integrate other geological datasets for enhanced analysis.

---

## **📜 Conclusion**
This project revealed significant insights into global seismic patterns, including magnitude-depth relationships, temporal trends, and geographic distributions. The findings provide a robust foundation for improving earthquake prediction, risk assessment, and resource allocation in seismology.

**Prepared by:**  
Adewole Oyediran  
📧 Email: Bensha2019@outlook.com
