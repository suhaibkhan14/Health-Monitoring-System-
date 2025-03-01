# 🚀 Health Monitoring System

## Introduction
The Health Monitoring System is designed to process and analyze patient health data using Big Data technologies (Hadoop and Spark). The system generates synthetic health records for 10,000 patients and performs statistical analysis on parameters such as Blood Pressure (BP), Sugar Level, Cholesterol, and Hemoglobin.

## Objective
- Generate 10,000 patient profiles with health parameters.
- Store and process patient data using Hadoop (HDFS, MapReduce).
- Implement Spark for faster data processing.
- Perform statistical analysis on health records.
- Visualize insights using Matplotlib/Tableau.

## Technologies Used
### Big Data Frameworks
- **Hadoop (HDFS, MapReduce):** Distributed storage and batch processing.
- **Spark (PySpark - Optional Extension):** Fast data processing.

### Programming Languages & Tools
- **Python:** Data generation, MapReduce scripting, and visualization.
- **HDFS (Hadoop Distributed File System):** Storing patient data.
- **Matplotlib & Tableau:** Visualization of health statistics.

## Implementation
### Generating Patient Data
A Python script generates synthetic patient records, storing them in a CSV file with the following attributes:
- **Patient_ID:** Unique identifier.
- **BP (Blood Pressure):** Systolic/Diastolic values.
- **Sugar Level:** Random glucose levels (mg/dL).
- **Cholesterol Level:** Cholesterol level (mg/dL).
- **Hemoglobin Level:** Hemoglobin count (g/dL).

### Storing Data in HDFS
The generated `patients.csv` file is uploaded to Hadoop HDFS using the following commands:
- **Create Directory:** `/health_monitoring`
- **Upload File:** `/health_monitoring/patients.csv`
- **List Directory:** `/health_monitoring/`

### Data Processing with Hadoop MapReduce
The Mapper extracts health attributes from each record and passes them to the Reducer for statistical calculations.

### Running MapReduce on Hadoop
Execute the MapReduce job using the Hadoop streaming jar.

### Data Visualization
Visualize the results using Matplotlib or Tableau to create insightful dashboards and charts.

## Conclusion
The Health Monitoring System successfully:
- Generated and stored 10,000 patient records.
- Used Hadoop (HDFS & MapReduce) for data processing.
- Computed health statistics using MapReduce.
- Visualized insights in a dashboard.

### Future Enhancements
- Implement Spark for real-time analysis.
- Deploy a web-based dashboard (Flask/Streamlit).
- Store data in NoSQL (MongoDB) for better scalability.

## References
- [Hadoop Official Docs](https://hadoop.apache.org/)
- [PySpark Guide](https://spark.apache.org/docs/latest/api/python/)
