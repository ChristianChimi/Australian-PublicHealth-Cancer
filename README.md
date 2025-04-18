Hi! This is a data analysis based on Australian public health database, cancer section.

Dataset source: https://data.gov.au/dataset/ds-dga-05696f6f-6ff5-42a2-904f-af5e4d1f56f8/details?q=cancer

Steps:
  - Pre-processing: drop NaN values for years where we don't hace cancer information.
  - Segmentation: Dividing Dataset into Incidence and Mortality Dataframes, also create a different DF for uterine cancer.
  - Data Reshaping: Melt and pivot uterine cancer by age (for clustering)

EDA:
  - Plot of cancer incidence and mortality by age.
  - Plotting normalized values of incidence
  - Calculating and plotting death ratio over the years.

Machine Learning/Statistics:
  - KMean to cluster similar groups by age dor uterine cancer.
  - ARIMA prediction of mortality and incidence for 5 future years
  - MLP: use deep learning to predict mortality ratio basing on incidence for every age group.
    The model learn which age group are more likely to die using incidence and death ratio, death ratio
    based on incidence on differents age group for the current year (given as input)
