# Aircraft Engine Sensor and Performance Analysis

## Project Overview

This project focuses on the analysis of aircraft turbofan engine sensor data using Python. The project uses the NASA C-MAPSS turbofan engine dataset to study sensor behaviour, operating-cycle patterns, relationships between sensors, and unusual sensor observations.

The analysis includes data preprocessing, descriptive statistics, correlation analysis, visualization, and statistical threshold-based anomaly detection.

## Objectives

- To collect and organize NASA C-MAPSS turbofan engine sensor data.
- To clean and validate the engine sensor dataset using Python.
- To calculate descriptive statistics for engine sensors.
- To analyse sensor behaviour across different operating cycles.
- To study relationships between sensors using Pearson correlation.
- To visualize sensor behaviour using different graphs.
- To identify unusual sensor observations using statistical thresholds.
- To compare sensor performance across different engine units.
- To interpret sensor patterns from an engineering perspective.
- To develop a reproducible data-analysis workflow for aircraft engine monitoring.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- NASA C-MAPSS Dataset

## Dataset

The project uses the NASA C-MAPSS Jet Engine Simulated Data.

The FD001 dataset contains:

- 100 engine units
- 20,631 records
- 3 operating settings
- 21 sensor measurements
- Operating-cycle information

Each record represents the operating condition of an engine during a particular operating cycle.

## Methodology

The project follows the following workflow:

NASA C-MAPSS Dataset  
↓  
Data Loading  
↓  
Data Cleaning and Validation  
↓  
Descriptive Statistical Analysis  
↓  
Sensor Correlation Analysis  
↓  
Time-Series Analysis  
↓  
Statistical Anomaly Detection  
↓  
Engine-Wise Comparison  
↓  
Engineering Interpretation

## Analysis Performed

### 1. Data Validation

The dataset is loaded using Pandas and checked for:

- Dataset dimensions
- Number of engine units
- Number of sensors
- Missing values
- Data structure

### 2. Descriptive Statistics

The following statistical measures are calculated:

- Mean
- Standard deviation
- Minimum value
- Maximum value
- Coefficient of variation

### 3. Correlation Analysis

Pearson correlation is used to identify relationships between different sensor measurements.

A correlation heatmap is generated to visualize the relationships between the sensors.

### 4. Time-Series Analysis

Sensor readings are plotted against operating cycles to study:

- Sensor trends
- Sensor fluctuations
- Gradual changes
- Unusual variations

### 5. Anomaly Detection

Potential unusual observations are identified using the statistical threshold:

Mean ± 3 × Standard Deviation

Observations outside this range are flagged for further engineering investigation.

### 6. Engine-Wise Comparison

Sensor measurements are grouped according to engine unit to compare:

- Average sensor values
- Sensor variation
- Operating behaviour
- Anomaly counts

## Visualizations

The project generates the following visualizations:

- Sensor time-series plots
- Sensor correlation heatmap
- Sensor box plots
- Engine-wise comparison charts
- Anomaly-count graphs

## Project Structure

Aircraft-Engine-Sensor-Analysis/

├── README.md  
├── train_FD001.txt  
├── aircraft_engine_analysis.py  
├── Aircraft_Engine_Analysis.ipynb  
│  
├── results/  
│   ├── correlation_heatmap.png  
│   ├── sensor_timeseries.png  
│   ├── sensor_boxplot.png  
│   └── engine_comparison.png  
│  
└── report/  
    └── Aircraft_Engine_Sensor_and_Performance_Analysis.pdf

## How to Run

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Aircraft-Engine-Sensor-Analysis.git
