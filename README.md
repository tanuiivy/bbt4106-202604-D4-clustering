# bbt4106-202604-D4-clustering

Group D4 submission for the K-means clustering lab.

## Team

**Name of the team on GitHub Classroom:**

### Member 1

| Details | Comment |
|---|---|
| **Student ID** | 168825 |
| **Name** | Wanyingi Shirleen Muthoni |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | I did Section 1 and 2: Data loading, EDA, and Feature Justification.<br>I learnt how to justify feature inclusion, exclusion and feature reserving. Excluding farmer_id was done because it is a unique identifier hence it is not meaningful for clustering. crop_type was reserved to be used for profiling after clusters are formed. I also learnt how to interpret visualizations for example histograms and boxplots to identify skewness and outliers.<br>Link to branch: https://github.com/tanuiivy/bbt4106-202604-D4-clustering/tree/feature/eda-shirleen|

### Member 2

| Details | Comment |
|---|---|
| **Student ID** | 166076 |
| **Name** | Angela Faith |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | I did section 2 : correlation and redundancy feature check and 3 : preprocessing pipeline (scaling and handling missing data). I learned the reasoning behind and how to identify features that might mislead an algorithm and possible ways of handling them. I also learned how to identify and categorise types of missingness in data and how to address each unique situation. Lastly I also learned the importance of scaling data and how to do it.

Link to branch: https://github.com/tanuiivy/bbt4106-202604-D4-clustering/edit/feature/preprocessing-Angela

### Member 3

| Details | Comment |
|---|---|
| **Student ID** | |
| **Name** | |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | |

### Member 4

| Details | Comment |
|---|---|
| **Student ID** | |
| **Name** | |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | |

### Member 5

| Details | Comment |
|---|---|
| **Student ID** | |
| **Name** | |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | |


## Video demonstration

Submit a link to a short video (5 minutes or less) demonstrating the
solution. Give the lecturer rights to view it. Submit the link only. Don't
upload the video file to the repository.

**Link to the video:**

## Repository structure

```
.
├── data/
│   └── agricultural_cooperative_farmers.csv
├── lab_submission/
│   └── bbt4106-202604-D4-clustering.ipynb
└── README.md
```

## Branch workflow

1. Create a branch from `main`, using the pattern `feature/<section>-<name>`.
   For example, `feature/eda-personA`.
2. Commit your section's work to your branch.
3. Open a pull request into `main` when your section is complete.
4. Read the full notebook after every merge. The individual defense can ask
   about any section, not only the one you wrote.
