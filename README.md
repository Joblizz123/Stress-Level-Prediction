# Stress-Level-Prediction
### INTRODUCTION
Considering today’s lifestyle, people just sleep forgetting the benefits sleep provides to the human body. Smart-Yoga Pillow (SaYoPillow) is proposed to help in understanding the relationship between stress and sleep and to fully materialize the idea of “Smart-Sleeping” by proposing an edge device (L. Rachakonda et. al, 2021). 

The dataset was sourced from kaggle. It is comprised of sleep-related features like snoring rate, respiration rate, temperature, limb movement rate, blood oxygen levels, eye movement, number of hours of sleep, heart rate and Stress levels. The Stress Levels are of four classes - 0 for low/normal, 1 for medium low, 2 for medium, 3 for medium high and 4 for high.

### EDA & VISUALIZATIONS
The dataset was analysed for missing values and duplicates. I also checked for outliers by using a descriptive statistics; there were no outliers, confirmed by using a box plot.

The relationship between the features and the label (Stress Levels) was also considered using Seaborn's  scatterplot. From the plot:
#### stress level increases with increase in:
- snoring rate
- respiration rate
- limb movement rate
- eye movement
#### and decreases with increase in:
- body temperature
- heart rate
I used Seaborn's FacetGrid to visualize the deistribution of the features.
### MODEL BUILDING 
The model was trained after splitting and scaling the dataset. I used hyperparameter tuning for three classifiers - Logistic Regression, Random Forest and Support Vector classifiers.

The model recorded 100% training accuracy and 99% for test accuracy.
Recall, Precision and F-1 scores were also calculated.
