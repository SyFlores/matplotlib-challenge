# matplotlib-challenge
This repository is intending to analyze data on pharmaceutical testing for mice, primarily using the matplotlib Python library.

*Collaborators: Sy Flores*

---
## **Table of Contents**
- [Abstract](#abstract)
- [Repository](#repository)
- [Body](#body)
  - [Data](#data)
  - [Methodology](#methodology)
- [Conclusion](#conclusion)
- [Sources](#sources)
---
## Abstract
We are intending to

## Repository
This section serves as a means to navigate the project/repository.
- **Data**
  - Mouse_metadata.csv
    - Houses data plainly describing the condition of the mouse at the start of the study, including the drug it has been assigned to
    - Includes the following fields: Mouse ID, Drug Regimen, Sex, Age_months, Weight (g)
  - Study_results.csv
    - Houses data obtained from study observations throughour treatment
    - Includes the following fields: Mouse ID, Timepoin, Tumor Volume (mm3), Metastatic Sites
- **Pymaceuticals**
  - Pymaceuticals.ipynb
    - This Jupyter Notebook serves as the primary script
    - This will largely display data manipulations and visualizations
  - Sources, Collaboration, and Thoughts.md
    - This md file will provide insight on thoughts, processes, and resources used during the project
- README.md
  - This .md file details most documentation needed in order to interpret the project
  - For code specific documentation, there are comments in the 'Pymaceuticals.ipynb' notebook detailing how the code functions

## Methodology
1. We will largely work to manipulate the data through merges, slices, and groupby's to put in the desired form
2. Using this transformed data, we will plot visualizations using Matplotlib
3. We will lastly perform a linear regression to show use alongside visualizations

## Conclusion
1. Both Capomulin and Ramicane initially appear to be the most effective Drug Regimen, having a much lower mean and variance than the other Drug Regimen.
2. Additionally, the first conclusion is strengthened because both Capomulin and Ramicane have the highest number of uses in the study. This may point to the two regimen being more effective at treating tumors as the mice are alive longer to track timepoints.
3. There does appear to be a strong correlation between mouse weight and tumor volume, with a correlation coefficent of approx. 0.8419.

---