# Racing Data Collection & Analysis
A Python toolkit for collecting, processing and analysing horse race data from UK and Ireland. This toolkit provides comprehensive data collection from Racing TV APIs and includes statistics to help identify fast-finishing horses. The toolkit also provides a summary of results for all of the horses racing today with further race day data collected from Racing Post APIs.

## 🏇 Features
- **Historical Data Collection:** Automated collection of horse racing data from Racing TV into a structured dataset
- **Current Day's Data:** Today's data collection from Racing Post APIs, useful for in race horse betting
- **Data Cleaning and Processing:** Data cleaning and grouping for each horse's performance history
- **Performance Analytics:** Summary statistics for each horse including statistics to help identify fast finishing horses

## ✅ Prerequisites
The code has only been tested using the following:
- Python 3.11.5
- Jupyter Notebook
- Stable internet connection for API calls
- Required Python packages (see `requirements.txt`)

## 🚦 Quick Start
### Get Today's Race Data
The process is fully automated - to get started simply run the `todays_data.ipynb` Jupyter Notebook.
#### **⚠️ Important Note**
**First-time setup or infrequent usage may take considerable time** - the system will automatically collect all missing data from the last date in the dataset to two days before today. This may require 30+ minutes for the initial run.

**Subsequent daily runs are much faster** - depending of wifi speed and stability, the code may take between 2-10 minutes each day.

## 📊 What You'll Get
### Today's Race Summary
The final outputs after running `todays_data.ipynb` include a CSV file and pandas DataFrame containing data for every horse racing today. More specifically, this includes
- Race day specific data
- Historical performance metrics for each horse
- Fast-finishing metrics for each horse
### 📷 Sample Output
<img width="3318" height="1306" alt="image" src="https://github.com/user-attachments/assets/b924ff1f-ff09-4575-8d85-239709ef8341" />

### 📄 Key Metrics Explained
The following metrics are all determined by the data in `historical_horse_data.json`.
#### Race Information
- **Track**: Name of the track for the race
- **Off Time**: The race's scheduled start time
- **Horse**: Name of the horse
- **Tips**: Number of race tips for that horse
#### Position Metrics
- **Best Pos**: Best position that the horse has achieved
- **Mean Pos**: Arithmetic mean of all the positions that the horse has achieved
- **Worst Pos**: Worst position that the horse has achieved
- **Std Pos**: Sample standard deviation of all the positions that the horse has achieved
#### Race Metrics
- **Num Wins**: Number of wins for that horse
- **Num Podiums**: Number of top three finishes for that horse
- **Num Fast Wins**: Number of High Fast Finishes for that horse
- **Num Races**: Number of races for that horse
#### Speed Metrics
- **High Fast Races (%)**: The percentage of races for which the horse's finishing speed was over 1 standard deviation above the above-median finishing speeds
- **Med Fast Races (%)**: The percentage of races for which the horse's finishing speed was over 0.8 standard deviation above the above-median finishing speeds
- **Low Fast Races (%)**: The percentage of races for which the horse's finishing speed was over 0.5 standard deviation above the above-median finishing speeds
- **Best Speed (mph)** The highest speed that the horse has achieved
