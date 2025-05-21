# Analyzing_Migration_in_Uttarakhand
Project Title: Analyzing the migration patterns in different district of Uttarakhand
Objective:
The aim of this project is to analyze various district-level socio-economic and environmental factors that influence rural-to-urban migration in Uttarakhand. The project builds a analyze model and visual dashboard to identify high-risk districts and key contributing factors to migration.
______________
Data Sources:
The data has been collected from multiple government reports and official datasets including:
•	Census Reports (2001, 2011)
•	Ministry of Agriculture (2015-2021)
•	IMD Rainfall Statistics
•	State Educational Statistics
•	Unemployment and Labor Participation from NSSO (where available)
All datasets are structured at the district level to allow for unified modeling.
______________
Key Features Used:
Agriculture:
•	Rabi and Kharif production, area, and yield
Household and Infrastructure:
•	Total households (rural/urban)
Rainfall:
•	Monthly rainfall
•	Annual rainfall and deviation from normal
Education:
•	Literacy Rate (2001, 2011)
•	Number of schools and colleges
Employment:
•	% of population in agriculture
•	Unemployment rate (where available)
Migration Data:
•	0–9 year recent migration counts from Census
•	Migration breakdown (ignored in modeling for simplicity)
______________
Methodology:
1.	Data Cleaning & Integration
o	Merged all datasets on district names
o	Handled missing values via mean imputation or domain-specific logic
2.	Feature Engineering
o	Created ratios (e.g., % rural households, % agricultural workers)
o	Normalized numerical columns for modeling
o	One-hot encoded categorical variables
3.	Exploratory Data Analysis (EDA)
o	Visualized correlations and skewness
o	Identified positive and negative indicators of migration
4.	Modeling
o	Firstly, we build the Linear regression model but its working is poor in our case so we switched to next model 
o	Applied Random Forest Regressor
o	Achieved R² score: 0.87, indicating good prediction quality
o	Validated with cross-validation
5.	Visualization Dashboard
o	Built in Power BI
o	Highlights:
	Migration area chart
	Unemployment rate
	Predicted migration rate vs. Actual migration rate
______________
Results & Interpretation:
•	Districts with low digitization, low literacy, and low agricultural productivity saw higher migration.
•	Rainfall deviation correlated moderately with migration trends in agriculture-heavy districts.
•	Skill development and education availability strongly correlated with lower migration.
______________
Key Takeaways:
•	Positive Factors: High literacy, stable agriculture, Good Healthcare facility
•	Negative Factors: Poor rainfall, low school/college density, No. of uninhabited villages
These insights can guide policy makers and development programs to target high-migration areas.
______________
Files Included:
•	/data/ folder with cleaned and raw data
•	model_training.ipynb with all preprocessing and modeling steps
•	PowerBI_Dashboard.pbix
•	README.md
______________
Author:
•	Kaushal Pandey, Nishant Tanwar, Priya Singhal
