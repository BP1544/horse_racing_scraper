# Racing Data Collection & Analysis
A Python toolkit for collecting, processing and analysing horse race data from UK and Ireland. This toolkit provides comprehensive data collection from Racing TV APIs and includes statistics to help identify fast-finishing horses. The toolkit also provides a summary of results for all of the horses racing today with further race day data collected from Racing Post APIs.

## 🏇 Features
- **Historical Data Collection:** Automated collection of horse racing data from Racing TV into a structured dataset
- **Current Day's Data:** Today's data collection from Racing Post APIs, useful for in race horse betting
- **Data Cleaning and Processing:** Data cleaning and grouping for each horse's performance history
- **Performance Analytics:** Summary statistics for each horse including statistics to help identify fast finishing horses

## 🚦 Quick Start
### Get Today's Race Data
The process is fully automated - to get started simply run the `todays_data.ipynb` Jupyter Notebook.
#### **⚠️ Important Note**
**First-time setup or infrequent usage may take considerable time** - the system will automatically collect all missing data from the last date in the dataset to two days before today. This may require 30+ minutes for the initial run.

**Subsequent daily runs are much faster** - depending of wifi speed and stability, the code may take between 2-10 minutes each day.
