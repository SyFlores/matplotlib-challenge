### Sources
- Question to be answered
  - Answer to question
    - Source: [Article name](Website URL)

### Collaborations
- No collaboration on this repository

### Thoughts
What is Being Asked? Pseudocode.

- Clean data
  - WiBA
    - Check the mouse ID's for any duplicate time points and remove those duplicate data points
  - Pc
    - Use df.drop_duplicates() to remove duplicate rows
- Summary statistics - tumor
  - WiBA
    - Generate a summary statistics table for the mean, median, variance, std dev, and SEM of the tumor volume for each drug regimen
  - Pc
    - Loop through a list of each drug regimen to generate the summary statistics and insert the drug regimen and statistic into a table
- Bar Plot - # of Measurements per Treatment Regimen
  - WiBA
    - Generate a bar plot showing the total number of measurements taken for each treatement regimen
  - Pc
    - Use Panda's DataFrame.plot() and Matplotlib's pyplot to plot
- Pie Plot - Gender Distribution
  - WiBA
    - Generate a pie plot showing the distribution of female or male mice in the study
  - Pc
    - Use Panda's DataFrame.plot() and Matplotlib's pyplot to plot
- Tumor Volume - Mouse across Treatment Regimens
  - WiBA
    - Calculate the final tumor volume of each mouse across the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin
    - Calculate the quartiles and IQR and quantitatively determine if there are any potential outliers across the four listed treatement regimen
  - Pc
    - Filter out the final timepoint (45) in Study_results
    - Join with Mouse_metdata on 'Mouse ID' and store in a DataFrame
    - Calculate quartiles and IQR for each drug regimen to define filter criteria
    - Add those to an outlier list for each of the four drug regimens
- Box and Whisker Plot - Tumor Volume by Treatment Regimens
  - WiBA
    - Create a box and whisker plot for each treatment regimen and highlight outliers
  - Pc
    - Create a box and whisker plot for the regimens on the same plot using the joined DataFrame
    - Check the Matplotlib documentation to style the outliers
- Line Plot - Capoumulin - Tumor Volume vs. Time Point
  - WiBA
    - Choose a mouse and plot a line plot of tumor volume vs time point
  - Pc
    - Plot a line plot using Study_results on any one mouse, plotting 'Tumor Volume (mm3)' against 'Timepoint'
- Scatter Plot - Capomulin - Weight vs. Average Tumor Volume
  - WiBA
    - Generate a scatter plot of mouse wieght versus average tumor volume for the Capomulin treatment region
  - Pc
    - Plot a scatter plot using joined DataFrame on any one mouse, plotting 'Weight (g)' against average 'Tumor Volume (mm3)'
- Corrlation Coefficient and LinReg Model - Capomulin - Mouse Weight and Average Tumor Volume
  - WiBA
    - Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment
    - Plot the linear regression model on top of the previous scatter plot
  - Pc
    - Do the functions!