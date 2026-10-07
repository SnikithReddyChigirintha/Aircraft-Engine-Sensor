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

How to Run

Step 1: Clone the Repository
git clone https://github.com/your-username/Aircraft-Engine-Sensor-Analysis.git

Step 2: Open the Project Folder
cd Aircraft-Engine-Sensor-Analysis

Step 3: Install Required Libraries
pip install pandas numpy matplotlib

Step 4: Add the Dataset
Place the following dataset file in the project directory:
train_FD001.txt

Step 5: Run the Python Program
python aircraft_engine_analysis.py

Results
The analysis provides a systematic approach to understanding aircraft engine sensor behaviour.
The project performs:
- Dataset validation
- Statistical analysis
- Correlation analysis
- Sensor time-series analysis
- Anomaly detection
- Engine-wise comparison
- Data visualization
The results provide a foundation for aircraft engine condition monitoring and future predictive-maintenance applications.

Future Scope

The project can be extended by:
- Implementing machine-learning models.
- Predicting Remaining Useful Life (RUL).
- Applying advanced anomaly-detection algorithms.
- Using real-time engine sensor data.
- Developing an interactive monitoring dashboard.
- Implementing deep-learning models such as LSTM.
- Comparing multiple C-MAPSS operating conditions.
- Developing an automated aircraft engine health-monitoring system.


Team Members

Roll Number	Name
25881A05DK	Student 1
25881A05CZ	Student 2
25881A05EB	Student 3
25881A05CB	Student 4


Academic Information

Course: Complex Engineering Problem 1 – Aerospace Engineering
Department: Computer Science and Engineering
Institution: Vardhaman College of Engineering
Academic Year: 2026–27

References

- NASA C-MAPSS Jet Engine Simulated Data
- Pandas Documentation
- NumPy Documentation
- Matplotlib Documentation
- Scikit-learn Documentation


Conclusion

The Aircraft Engine Sensor and Performance Analysis project demonstrates how Python-based data analytics can be used to study aircraft engine sensor data, identify unusual observations, and understand performance behaviour across operating cycles.
The developed workflow provides an interpretable foundation for engine condition monitoring, anomaly detection, and future predictive-maintenance systems.
