# Data Mining Project - University of Pisa, Academic Year 2023/24

## Authors
- Giacomo Aru
- Giulia Ghisolfi
- Luca Marini
- Irene Testa

## Dataset Description
The project utilizes three CSV files:

1. **incidents.csv:** Contains information about gun incidents in the USA.
   - Variables include date, state, city_or_county, address, latitude, longitude, congressional_district, state_house_district, and more.
   - Additional features: participant_age_group1, participant_gender1, n_killed, n_injured, notes, incident_characteristics1, incident_characteristics2.

2. **povertyByStateYear.csv:** Provides poverty percentages for each USA state and year.
   - Variables include state, year, and povertyPercentage.

3. **year_state_district_house.csv:** Presents details about the winner of congressional elections in the USA.
   - Variables include year, state, congressional_district, party, candidateVotes, and totalVotes.

## Task 1: Data Understanding and Preparation (30 points)

### Task 1.1: Data Understanding
Explore the incidents dataset using analytical tools, assessing data quality, variable distribution, and pairwise correlations.

### Task 1.2: Data Preparation
Improve data quality and extract new features. Define indicators such as:
- Males involved in incidents relative to the total number of males in the same city and period.
- Ratio of killed people to participants in incidents.
- Ratio of unharmed people in incidents relative to the average in the same period.

## Subtasks of Data Understanding:
- Define data semantics for each feature.
- Examine variable distribution and statistics.
- Assess data quality (missing values, outliers, duplicates, errors).
- Perform variable transformations.
- Explore pairwise correlations and eliminate redundant variables.
- Visualize insights using latitude and longitude features (e.g., with [Plotly](https://plotly.com/python/getting-started/)).

## Task 2: Clustering Analysis (30 points - 32 with optional subtask)

Explore the dataset using various clustering techniques based on the extracted features.

### Subtasks:

1. **K-means Clustering on the Entire Dataset:**
   - Identify the best value of k.
   - Characterize obtained clusters using analysis of k centroids and comparison of variable distributions.
   - Evaluate clustering results.

2. **Density-Based Clustering:**
   - Select one state in the dataset.
   - Study clustering parameters.
   - Characterize and interpret obtained clusters.

3. **Hierarchical Clustering:**
   - Choose one state in the dataset.
   - Compare clustering results using different versions of the algorithm.
   - Show and discuss different dendrograms using various algorithms.

4. **Final Evaluation:**
   - Evaluate the best clustering approach and compare obtained clusters.

5. **Optional (2 points):**
   - Explore alternative clustering techniques using the [pyclustering](https://github.com/annoviko/pyclustering/) library.
