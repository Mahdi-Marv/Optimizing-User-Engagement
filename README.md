# README for HW-02.ipynb

## Overview
This Jupyter Notebook performs statistical data analysis with a focus on A/B testing methodologies applied to news headlines from Upworthy. The primary goal is to analyze how different headlines affect user engagement and click rates.

## Course Information
- **Course Title:** Foundations of Data Science
- **Instructor:** Dr. Khalaj
- **Term:** Fall 2023


## Objectives
1.  Utilize advanced practices in Numpy, Pandas, and Matplotlib.
2.  Conduct simple statistical analyses on the provided dataset.
3.  Generalize findings to suggest improvements for Upworthy's performance.
4.  Discuss potential solutions to maximize user engagement through headline selection.

## Data Source
The data used in this assignment is derived from a research paper available [here](https://doi.org/10.1038/s41597-021-00934-7) and is located in the `data` folder of the project as `upworthy.csv`.

## Data Description
The dataset contains the following columns:

| Column Name          | Description                                                                                                                                    |
|----------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| created_at           | Time the package was created (timezone unknown)                                                                                             |
| test_week            | Week the package was created, used for stratified random sampling                                                                            |
| clickability_test_id | The test ID for random assignment of viewers to packages                                                                                     |
| impressions          | Number of viewers assigned to this package                                                                                                   |
| headline             | The headline being tested                                                                                                                    |
| eyecatcher_id        | Image ID associated with the package                                                                                                         |
| clicks               | Number of clicks on the package                                                                                                             |
| excerpt              | Excerpt of the article                                                                                                                       |
| lede                 | Opening sentence or paragraph of the story                                                                                                   |
| slug                 | Internal name for the web address                                                                                                            |
| share_text           | Summary for social media sharing                                                                                                             |
| square               | Part of the social media sharing suggestion                                                                                                   |
| significance         | A complex calculation comparing clicks on a package to previous packages on the same pages                                                   |
| first_place          | Indicator shown to editors to guide decisions about which test to choose                                                                      |
| winner               | Indicates whether a package was selected for use on the Upworthy site after testing                                                          |
| updated_at           | Last time the package was updated in the Upworthy system                                                                                     |

## Analysis Steps
1.  **Data Loading**: The notebook begins by importing necessary libraries such as NumPy, Pandas, Matplotlib, and Seaborn. It then loads the dataset using `pd.read_csv()`.
2.  **Experiment Analysis**: The notebook calculates:
    *   The total number of different experiments conducted (4822).
    *   The average number of packages considered per experiment (approximately 4.27).
3.  **Visualization**: The notebook includes a section for plotting the distribution of packages per experiment.

## Requirements
To run this notebook, ensure you have the following Python packages installed:

-   numpy
-   pandas
-   matplotlib
-   seaborn

You can install these packages using pip:

```bash
pip install numpy pandas matplotlib seaborn
