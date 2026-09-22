# INFO 2950 Project: Sleep and Health

Semester project for INFO 2950: Introduction to Data Science at Cornell University, Fall 2026.

## Team

- Eric Wang
- Mary Yang

## Current Status

Phase I: Project Brainstorming. We are considering the three ideas below; the final topic has not been selected. Data collection and analysis have not yet begun.

## Candidate Ideas

### 1. Weekend Catch-Up Sleep and Depressive Symptoms

Among adults who usually sleep fewer than seven hours on workdays, is sleeping longer on non-workdays associated with depressive symptom scores?

We propose combining the NHANES 2017-2018 Sleep Disorders (`SLQ_J`), Depression Screener (`DPQ_J`), and Demographics (`DEMO_J`) files using participant identifier `SEQN`.

### 2. Physical Activity, Sedentary Time, and Sleep Duration

How are recreational physical activity and sedentary time associated with workday sleep duration among adults?

We propose combining the NHANES 2017-2018 Sleep Disorders (`SLQ_J`), Physical Activity (`PAQ_J`), and Demographics (`DEMO_J`) files using `SEQN`.

For Ideas 1 and 2, we will ask our mentors whether combining distinct modules within NHANES meets the course's data sourcing requirement.

### 3. County Economic Conditions and Insufficient Sleep

Do counties with lower household incomes or higher poverty rates have higher estimated prevalence of insufficient sleep?

We propose combining CDC PLACES county-level sleep estimates with 2018-2022 American Community Survey five-year income and poverty estimates using five-digit county FIPS codes. We will verify geographic and time-period compatibility. Because PLACES modeling already incorporates poverty and demographic information, we will seek mentor guidance on this limitation before selecting the topic.

## Data Sources

- [NHANES 2017-2018 data directory](https://wwwn.cdc.gov/Nchs/Nhanes/Search/DataPage.aspx?Cycle=2017-2018)
- [CDC PLACES](https://www.cdc.gov/places/)
- [Census data download portal](https://data.census.gov/)
- [ACS 2022 five-year income table B19013 documentation](https://api.census.gov/data/2022/acs/acs5/groups/B19013.html)
- [ACS 2022 five-year poverty table B17001 documentation](https://api.census.gov/data/2022/acs/acs5/groups/B17001.html)

## Repository Structure

```text
INFO-2950-Project/
|-- README.md
|-- data/
|   |-- raw/
|   `-- processed/
|-- notebooks/
`-- reports/
    `-- phase1/
```

- `data/raw/`: Original source data, preserved without edits.
- `data/processed/`: Cleaned, analysis-ready datasets generated from raw data.
- `notebooks/`: Data cleaning, exploratory analysis, and modeling notebooks.
- `reports/phase1/`: Phase I proposal and submission files.

Empty directories contain `.gitkeep` files so Git can track the structure. Detailed collection instructions and dependencies will be added once a topic is selected.

## Collaboration

Pull the latest changes before working and use descriptive commit messages. Coordinate before editing the same notebook to reduce merge conflicts. Keep data cleaning in a separate notebook that outputs the data used by the analysis notebooks.
