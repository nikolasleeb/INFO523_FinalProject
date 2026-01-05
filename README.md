# Final Project for INFO 523 - Data Mining/Discovery

## Fall '25 MS of DS @ University of Arizona

---

### Project Description

 The goal of this project was to explore two data driven questions using the techniques we learned across the semester. The two questions I wanted to ask were:
    1. Using historical vehicle registrations, fuel efficiency, and gasoline consumption, can we accurately predict future gasoline consumption?
       * This question is based upon the INFO 511 project that I completed earlier in the semester and the ideas for improvements that I had.
    2. Do Gasoline and Diesel prices within the U.S. move in similar ways and based upon the movement of one, can we predict the other?

    I began exploring the first question by cleaning the datasets and merging them together. I then used a correlation matrix to see which variables were best correlated to gasoline consumption. From this, I decided that licensed drivers and average fuel economy were going to be our predictors of gasoline consumption. We then tested different models and methods including Principal Component Analysis(PCA), Walk-Forward Validation, XGBoost, and GridSearch to try to predict gasoline consumption in the future. One problem that we ran into was that our original time span was 1995-2021, but the data from November 2019 - May 2021 does not follow historical trends due to COVID-19. Because of this, we decided to change our time span to end in 2019.

    To answer the second question, I again began by cleaning our dataset. To check if gasoline and diesel prices moved similary and could be used to predict the other, I decided to use a couple of different methods. The first was to run a correlation test to check if gasoline and diesel prices were highly correlated to one another. I then used a linear regression model to check the variance. Following that we used some visualizations including line plots, heatmaps, and bar charts. The bar chart was used to show how many months the prices moved in the same direction, the heat map was used to show when the prices were within a 5% range of other, and the line plots were used to show both of the those same trends but in a different way. The visualizations and results were then aggregated into a dashboard. 

---

### Project Requirements

[Project Requirements Document in Google Drive](https://drive.google.com/file/d/1H5ssxc3-JyBZK2CLcOc8Wy99x778WMtz/view?usp=sharin)

Step 1. Project Proposal
Step 2. Project Analysis and Development
Step 3. Write FinalReport

---

### Project Breakdown

```text
|---FEVRC_Analysis
|   |---Images Folder
|   |---FEVRC_Dataset.csv
|   |---FEVRC_Notebook.ipynb
|
|---FP_Analysis
|   |---Images Folder
|   |---FP_Notebook.ipynb
|
|---FuelConsumption
|   |---RAW Folder (raw imported data)
|   |---cleanedconsumption.csv
|   |---ConsumptionData.ipynb
|   |---ConsumptionData.xlsx
|
|---FuelEconomy
|   |---RAW Folder (raw imported data)
|   |---cleanedfueleconomy.csv
|   |---FuelEconomy.ipynb
|   |---FuelEconomy.xlsx
|
|---FuelPrices
|   |---RAW Folder (raw imported data)
|   |---cleanedprices.csv
|   |---FuelPrices.ipynb
|   |---MonthlyRetailPrices.xlsx
|
|---VehicleRegistrations
|   |---RAW Folder (raw imported data)
|   |---cleanedregistrations.csv
|   |---VehicleRegistration.ipynb
|   |---VehicleRegistrations.xlsx
|
|---ProjectDocuments
|   |---INFO523_FinalProjectGuidelines.pdf
|   |---ProjectProposal.docx
|
|---FinalReport.docx
```

---

### Ideas for Improvement
