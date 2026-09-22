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
| **Student ID** | |
| **Name** | |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | |

### Member 3

| Details | Comment |
|---|---|
| **Student ID** |166918 |
| **Name** |Kariuki Irene Wanjiru |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | Completed sections 5 and 6: I compared four cluster validity metrics (inertia, silhouette, Davies-Bouldin, and Calinski-Harabasz) across k=2 to 10 on the scaled clustering features. I found the metrics disagree: the elbow method points to k=5–6, while silhouette, Davies-Bouldin, and Calinski-Harabasz all favor k=2, which I attributed to farm size and yield's strong right-skew making a coarse "large vs. smallholder" split easy to separate cleanly. I then ran cluster diagnostics on four candidate values (k=2, 4, 5, and 6), confirming no near-empty or imbalanced clusters at any of them, and I interpreted the silhouette scores (0.52 at k=2 vs. 0.29–0.31 for k=4–6) to frame the trade-off between statistical optimality and practical usefulness for the final k justification.<br>Link to branch: https://github.com/tanuiivy/bbt4106-202604-D4-clustering/tree/faeture/determining-k-Irene|

### Member 4

| Details | Comment |
|---|---|
| **Student ID** | 164430|
| **Name** |Maxwell Gitonga |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** |Completed sections 7 and 8: justifying the final chosen k and the robustness check. All three validity metrics (silhouette, Davies-Bouldin, Calinski-Harabasz) mathematically favored k=2, but profiling showed k=2 only separated farmers by farm size — a split already visible without clustering. k=5 preserved that same large-scale farming cluster while splitting smallholders into four distinct, actionable profiles differing in income per acre, market access, and experience, so I chose k=5 over the statistically "best" k=2 for business interpretability. I then confirmed the k=5 solution was robust to a different random seed (Adjusted Rand Index = 0.98) and to an alternative scaling method, MinMaxScaler instead of StandardScaler (ARI = 0.84). I learned that the statistically top-scoring solution isn't automatically the right one to report — validity metrics need to be weighed against whether the resulting clusters are actually useful for the business question being asked.<br>Link to branch: https://github.com/tanuiivy/bbt4106-202604-D4-clustering/tree/feature/robustness-maxwell |

### Member 5

| Details | Comment |
|---|---|
| **Student ID** | 153130 |
| **Name** |Ivy Tanui |
| **What part of the lab did you personally contribute to (provide a link to the branch(es)), and what did you learn from it?** | Completed sections 9–11: cluster profiling, model persistence, and the final academic/business report. For profiling, I used group-wise means and a crop_type cross-tabulation to name and interpret all five clusters, then wrote the report in the format of the class demo but with our own numbers and findings. For persistence, I saved the fitted scaler and clustering model together and demonstrated a prediction on a new manually-built farmer. I learned that k = 2 scored better on every validity metric we tested, but we chose k = 5 anyway because it reveals structure a two-cluster split completely hides, which showed me the "best" statistical score isn't always the most useful one for the business question. <br>Link to branch: https://github.com/tanuiivy/bbt4106-202604-D4-clustering/tree/feature/profiling-ivy|


## Video demonstration

Submit a link to a short video (5 minutes or less) demonstrating the
solution. Give the lecturer rights to view it. Submit the link only. Don't
upload the video file to the repository.

**Link to the video:** https://docs.google.com/videos/d/1ZEHy_gTWTeOf9hn86tIZoBJUlle-5IVtFNXLA16853I/play?usp=sharing

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
