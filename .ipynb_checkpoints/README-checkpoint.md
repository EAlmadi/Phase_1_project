
Aircraft Analysis Project
Business Problem
Your company is expanding into new industries to diversify its investment portfolio. One of the target sectors is aviation, specifically purchasing and operating aircraft for both commercial and private use.

However, the company currently lacks knowledge about the risks associated with different aircraft types.

Objective:
You have been tasked with analyzing historical aircraft incident and crash data to identify the lowest-risk aircraft for investment. Your findings will provide actionable insights to guide the company's purchasing decisions.

Project Goal
Identify low-risk aircraft for my client to invest in.

Approach & Plan
I plan to follow the steps below:

Import Necessary Libraries

Use pandas for data manipulation
Use matplotlib.pyplot for data visualization
Load the Dataset

Read the CSV file into a DataFrame
Preview the first few rows using .head()
Understand the Data

Use .info(), .describe(), and .isna().sum() to examine data types, null values, and distributions
Identify key columns for analysis (e.g., aircraft make, fatalities, weather conditions, damage)
Clean the Data

Handle missing or inconsistent data
Convert data types where needed
Standardize text and remove duplicates
Perform Exploratory Data Analysis (EDA)

Visualize trends such as:
Most and least risky aircraft
Fatalities and destruction rates by aircraft make
Incidents over time and weather-related crashes
Draw Conclusions

Summarize which aircraft makes are associated with low or high risk
Provide Recommendations

Identify the safest aircraft makes for investment
Suggest aircraft makes to avoid or investigate further n Libraries**
`Data Cleaning
Goal:
To prepare the dataset for analysis by ensuring consistency, handling missing data, and organizing the structure for efficient exploration.

Steps:
.info()

View a summary of the DataFrame.
Check:
Number of non-null values
Data types
Column names
Shape (rows and columns)
.isna().sum()

Identify columns with missing values.
Count how many missing values exist per column.
.describe()

Generate summary statistics (mean, median, std, min, max, etc.) for numerical columns.
.sort_values()

Sort data in ascending or descending order.
Useful for identifying extremes (e.g., highest fatalities or destruction rates).
Fixing Data Types

Convert columns to appropriate types (e.g., dates to datetime, numeric strings to integers/floats).
Standardizing Text

Clean text columns (e.g., make all text lowercase, remove whitespace).
Useful for grouping and comparison.
Checking for Duplicates

Use .duplicated() and .drop_duplicates() to remove duplicate rows that may affect analysis accuracy.
Once the data is cleaned and structured, it will be ready for effective exploratory data analysis (EDA).

Visualizations Using Matplotlib
Visualizing aircraft crash data using matplotlib makes complex patterns easier to understand. It helps in decision-making and reveals important trends and patterns related to aviation safety.

1. Aircraft Makes Most Likely to Be Destroyed
This bar chart shows the top 10 aircraft makes with the highest destruction rate in crashes.

A higher destruction rate may indicate weaker structural integrity or higher-risk operating environments.
2. Aircraft Makes Least Likely to Be Destroyed
These aircraft makes have the lowest destruction rates, which likely means:

They are more durable, or
Involved in fewer severe accidents.
This visualization helps identify potentially safer investment options.

3. Aircraft with the Most Incidents
This bar chart highlights the aircraft makes with the highest number of recorded incidents.

A high number may suggest:
Maintenance issues
Poor safety records
Or simply greater popularity (more planes in service).
4. Aircraft with the Most Fatalities
Displays aircraft makes associated with the highest total fatalities.

This is critical for identifying aircraft with poor survivability in crashes.
5. Aircraft with the Least Fatalities
Shows aircraft makes with the lowest non-zero fatality counts.

Aircraft with 0 fatalities were excluded.
Helps identify safer aircraft models.
6. Crashes Influenced by Weather Conditions
Analyzes the number of crashes where weather played a role.

Important for assessing environmental risk factors.
7. Number of Aircraft Incidents per Year
A time-series plot showing how incidents have changed annually.

Useful for spotting trends or improvements in safety over time.
8. Aircraft Incidents by Weather Condition Over the Years
Combines weather categories with time to show:

Weather-related incident trends
Seasonal or climate-based risk factors
9. Number of Fatalities per Incident
Calculates the fatality rate per crash.

Helps differentiate between:
High-fatality, low-frequency incidents
Low-fatality, high-frequency incidents
10. Fatalities Over Time by Aircraft Make
A historical look at fatalities over time, grouped by aircraft make.

Shows which makes are consistently safer or riskier over the years.
Summary: These visualizations help uncover patterns, guide aviation safety policy, and inform aircraft investment or regulatory decisions.
Key Findings
Cessna and Piper had the highest number of incidents, suggesting either high operational exposure or potential safety concerns.
Kenetic Aviation and Mcnicholas had very few incidents and no recorded fatalities or destruction, making them strong candidates for low-risk investment.
Beech and Boeing showed relatively high fatality counts, which may warrant caution when considering these aircraft makes.
Aircraft damage analysis revealed that certain makes are more likely to be completely destroyed in crashes, potentially indicating weaker structural integrity or safety performance.
Destruction rate analysis highlighted aircraft makes that consistently fared better in crash survivability, which is a valuable indicator of safer design.
Conclusion
Based on the analysis of incident data, fatality rates, and destruction rates, it is evident that not all aircraft makes carry the same level of risk.

Aircraft makes such as Kenetic Aviation, Mcnicholas, and Mcnabb consistently demonstrated low risk, with few incidents, no recorded fatalities, and minimal or no destruction in crashes. These makes may be considered ideal starting points for the company’s investment.

In contrast, makes such as Cessna, Piper, and Beech, while popular, were involved in a high number of incidents and exhibited significant fatalities and destruction rates. These should be approached with caution or subjected to further investigation before any investment decision is made.

By combining historical safety data with business strategy, I recommend the company prioritize aircraft makes that show:

Low incident counts
Minimal destruction rates
Few or no recorded fatalities
These insights provide a foundation for safer, evidence-based decisions as the company enters the aviation industry.

Recommendations
Start with Safer Aircraft Makes
Focus on aircraft like Kenetic Aviation, Mcnicholas, and Mcnabb which had the fewest incidents and no recorded fatalities.

Avoid High-Risk Makes for Now
Be cautious with makes such as Cessna, Piper, and Beech, which had higher incident and fatality rates.

Use Safety Data to Guide Purchases
Always review historical safety data—such as incident counts and destruction rates—before buying any aircraft.




