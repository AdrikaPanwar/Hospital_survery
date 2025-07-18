 # Hospital Survey (Data Analyst Intern Assessment - Adagama Digital)

#### Project Overview
This project focuses on analyzing a healthcare and provider survey dataset obtained from Kaggle. The dataset comprises multiple CSV files and a data dictionary (.csv and .xlsx formats), capturing:
- Hospital ratings
- Patient experience scores
- Demographic insights
The objective is to clean, model, and visualize the data using Python (Pandas) for cleaning and Tableau for interactive dashboards and KPI reporting.

<img width="1062" alt="Screenshot 2025-06-13 at 4 28 29 PM" src="https://github.com/user-attachments/assets/4da1f70a-ab90-4c3f-b24b-c74991728939" />
<img width="1425" alt="Screenshot 2025-06-13 at 2 38 27 AM" src="https://github.com/user-attachments/assets/42b39b36-c645-45f0-801e-7bb87734a733" />


## Files Used for Visualization
Note: File names were renamed as per convenience.
| Original File     | Renamed As    |
| ----------------- | ------------- |
| `measures.csv`    | `measures`    |
| `national.csv`    | `national`    |
| `questions.csv`   | `questions`   |
| `reports.csv`     | `reports`     |
| `state.csv`       | `state`       |
| `responses.csv`   | `responses`   |
| `states_cont.csv` | `states_cont` |
| `data_dict`       | `data names`  |

Each dataset is linked using unique IDs, as shown below:

## Relationship Between Tables
| .csv file    | unique\_id 1   | unique\_id 2      |
| ------------ | -------------- | ----------------- |
| measures     | Measure ID     |                   |
| national     | Measure ID     |                   |
| reports      | Release Period |                   |
| questions    | Measure ID     |                   |
| responses    | Release Period | state             |
| state        | Release Period | state, Measure ID |
| states\_cont | state          |                   |

```state.csv``` also contains Measure ID not mentioned above.

And for more Detail must read this https://github.com/AdrikaPanwar/Hospital_survery/blob/main/arth_report.pdf

## How to Run Locally
Clone the repository
```
git clone https://github.com/AdrikaPanwar/Hospital_survey.git
cd Hospital-Survey-Analysis
```

## Install required packages
```
pip install pandas matplotlib seaborn jupyter
```
Run Notebooks
- Start with: ```Hospital_survey.ipynb```
- Check logic, schema design, and cleaning operations.

---

## Thanks for Reading this

