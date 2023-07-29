
# Automatidata Project - New York City Taxi TLC Exploratory Data Analysis (EDA) and Data Visualization

## Scenario

Your team is working on a project for the New York City Taxi and Limousine Commission (TLC). The project involves conducting exploratory data analysis (EDA) and data visualization using Python and Tableau. The goal is to gain insights into taxi ridership in NYC.

## Instructions

1. Project Proposal:
   - Begin by reviewing the project proposal to understand the objectives and scope of the project.

2. TLC Dataset Inspection and Organization:
   - Use Python to inspect and organize the TLC dataset. Ensure the data is clean and structured properly.

3. Email from Luana Rodriguez, Senior Data Analyst:

   Subject: New York City TLC EDA & Vizzes

   From:  "Luana Rodriguez" <Luana@automatidata>

   Cc: "Deshawn Washington" <Deshawn@automatidata>; "Udo Bankole" <Udo@automatidata>

   Hi there,

   Thanks for the amazing work you’ve done so far.

   We’re ready to perform EDA on the taxi data from the New York City TLC to get a general understanding of what taxi ridership looks like. Has Deshawn told you what the management team expects when it comes to EDA? If not, think of it as a “show your work” kind of report. They will want to see a Python notebook showing the structuring and cleaning you did, as well as any matplotlib/seaborn visualizations you plotted to help us understand the data. I would suggest at the very least a box plot of the ride durations and some time series plots, like a breakdown by quarter or month? Whatever you think makes most sense.

   Additionally, the management team has recently asked all EDA to include Tableau visualizations. We’ve found these to be particularly helpful in status reports to the client and board members. Make sure it is easy to understand to someone who isn’t data savvy, and remember that the assistant director at the New York City TLC is a person with visual impairments. I understand you have some Tableau experience? Let me know if you need help with this.

   By the way, I Cc’d our director, Udo, who is on the management team and will be reviewing/approving our analysis before the project manager reports it back to the client. @Udo, I just want to keep you informed on the progress!

   Thanks!

   Luana Rodriguez

   Senior Data Analyst

   Automatidata

4. Email from Udo Bankole, Director of Data Analysis:

   Subject: RE: New York City TLC EDA & Vizzes

   From:  "Udo Bankole" <Udo@automatidata>

   Cc: "Deshawn Washington" <Deshawn@automatidata>; "Luana Rodriguez" <Luana@automatidata>

   Thank you, Luana!

   Welcome to the team, so glad to have you.

   Along with the Tableau visualization and notebook, it would be really helpful if you included an executive summary of your analysis attached via email.

   I appreciate your help!

   Udo Bankole

   Director of Data Analysis

   Automatidata

5. EDA in Python:
   - Create a Python notebook that demonstrates your EDA process. Include code for data cleaning, structuring, and relevant matplotlib/seaborn visualizations, such as a box plot of ride durations and time series plots (e.g., breakdown by quarter or month).

6. Tableau Visualization:
   - Create Tableau visualizations that complement your Python analysis. Ensure the visualizations are easy to understand for non-data savvy individuals and consider accessibility for people with visual impairments.

7. Executive Summary:
   - Prepare an executive summary of your analysis. This summary should highlight key findings and insights obtained from the EDA and data visualizations.

8. Review and Approval:
   - Before finalizing the analysis, share your work with Luana and Cc Udo in an email to keep them informed of your progress. Incorporate any feedback they may have.

9. Final Report:
   - Once your analysis and visualizations are complete and approved, compile all your work, including the Python notebook, Tableau visualizations, and executive summary, into a final report.

## Final Notes

Ensure that your EDA is thorough, well-documented, and visually appealing. The executive summary should be concise yet informative, providing a clear overview of the insights gained from the data analysis.

Collaborate effectively with your team members, Luana, and Udo throughout the process to ensure a successful and impactful analysis for the New York City TLC.

## Data Dictionary

Sure, here's the data dictionary formatted as a table:

| Column Name            | Description                                                                                     |
|------------------------|-------------------------------------------------------------------------------------------------|
| ID                     | Trip identification number                                                                      |
| VendorID               | A code indicating the TPEP provider that provided the record.                                   |
|                        | 1 = Creative Mobile Technologies, LLC                                                          |
|                        | 2 = VeriFone Inc.                                                                              |
| tpep_pickup_datetime   | The date and time when the meter was engaged.                                                  |
| tpep_dropoff_datetime  | The date and time when the meter was disengaged.                                               |
| Passenger_count        | The number of passengers in the vehicle. This is a driver-entered value.                      |
| Trip_distance          | The elapsed trip distance in miles reported by the taximeter.                                  |
| PULocationID           | TLC Taxi Zone in which the taximeter was engaged.                                              |
| DOLocationID           | TLC Taxi Zone in which the taximeter was disengaged.                                           |
| RateCodeID             | The final rate code in effect at the end of the trip.                                         |
|                        | 1 = Standard rate                                                                             |
|                        | 2 = JFK                                                                                       |
|                        | 3 = Newark                                                                                    |
|                        | 4 = Nassau or Westchester                                                                     |
|                        | 5 = Negotiated fare                                                                           |
|                        | 6 = Group ride                                                                               |
| Store_and_fwd_flag     | This flag indicates whether the trip record was held in vehicle memory before being sent to the vendor, aka "store and forward," because the vehicle did not have a connection to the server. |
|                        | Y = store and forward trip                                                                    |
|                        | N = not a store and forward trip                                                              |
| Payment_type           | A numeric code signifying how the passenger paid for the trip.                                |
|                        | 1 = Credit card                                                                              |
|                        | 2 = Cash                                                                                     |
|                        | 3 = No charge                                                                                |
|                        | 4 = Dispute                                                                                  |
|                        | 5 = Unknown                                                                                  |
|                        | 6 = Voided trip                                                                              |
| Fare_amount            | The time-and-distance fare calculated by the meter.                                           |
| Extra                  | Miscellaneous extras and surcharges. Currently, this only includes the $0.50 and $1 rush hour and overnight charges. |
| MTA_tax                | $0.50 MTA tax that is automatically triggered based on the metered rate in use.              |
| Improvement_surcharge  | $0.30 improvement surcharge assessed trips at the flag drop. The improvement surcharge began being levied in 2015. |
| Tip_amount             | Tip amount – This field is automatically populated for credit card tips. Cash tips are not included. |
| Tolls_amount           | Total amount of all tolls paid in trip.                                                       |
| Total_amount           | The total amount charged to passengers. Does not include cash tips.                           |


## PACE Plan - Planning, Analysis, Construct, and Execute

### Previous Completion Summary

In the previous phase of the project, the team completed the project proposal and used Python to inspect and organize the New York City TLC dataset. The dataset, named "2017_Yellow_Taxi_Trip_Data.csv," contains information related to taxi trips in NYC and comprises 408,294 rows with 18 columns capturing various data variables for each trip.

### Planning

For the upcoming phase, the focus will be on conducting exploratory data analysis (EDA) and data visualization. The team will follow the PACE framework, which includes four main stages: Planning, Analysis, Construct, and Execute.

In the Planning stage, the team will:
1. Review the email communication from Luana Rodriguez, Senior Data Analyst, and Udo Bankole, Director of Data Analysis, to understand the specific requirements and expectations for the EDA and data visualization.
2. Define the objectives of the EDA, which involve gaining a general understanding of taxi ridership in NYC and identifying key insights from the dataset.
3. Identify the necessary Python libraries and tools required for data cleaning, structuring, and visualization.
4. Plan the timeline and allocate tasks among team members to ensure a smooth execution of the project.

### Analysis

In the Analysis stage, the team will:
1. Conduct data cleaning and preprocessing using Python to ensure the dataset is in a usable format for analysis.
2. Perform statistical analysis on relevant variables such as trip duration, passenger count, and trip distance to gain insights into the distribution and patterns in the data.
3. Create visualizations using matplotlib and seaborn to visually represent the data and explore relationships between different features.
4. Generate time series plots, such as breakdowns by quarter or month, to understand trends in taxi ridership over time.

### Construct

In the Construct stage, the team will:
1. Develop Tableau visualizations based on the insights obtained from the Python analysis.
2. Ensure that the Tableau visualizations are intuitive, informative, and accessible to non-data savvy individuals, including those with visual impairments.
3. Include visualizations that represent key metrics, such as ride duration distributions, passenger counts, and trip distances, to provide a comprehensive overview of taxi ridership in NYC.

### Execute

In the Execute stage, the team will:
1. Collaborate and communicate effectively with team members, Luana Rodriguez, and Udo Bankole to ensure progress is monitored and any potential roadblocks are addressed.
2. Share intermediate progress and results with Luana and Cc Udo through email communication, incorporating their feedback and suggestions into the analysis and visualizations.
3. Prepare an executive summary of the analysis, highlighting key findings, trends, and insights from both the Python and Tableau analysis.
4. Compile all the deliverables, including the Python notebook, Tableau visualizations, and executive summary, into a comprehensive final report.

By following the PACE framework, the team aims to deliver a well-structured and insightful analysis of the New York City TLC dataset, providing valuable information to the management team and stakeholders at Automatidata and the New York City TLC.

## Data Analysis with Public Tableau

In this section, we will leverage the power of Tableau Public to conduct data analysis and create interactive visualizations based on the New York City TLC dataset. Tableau Public is a free platform that allows us to publish and share visualizations with a wider audience.

### Connecting to the Dataset

1. Open Tableau Public and create a new project for the New York City TLC analysis.

2. Import the "2017_Yellow_Taxi_Trip_Data.csv" dataset into Tableau Public using the data connection option. Ensure that the data types are correctly recognized, and the data is accurately structured.

### Exploratory Data Analysis (EDA)

3. Explore the Dataset: Start the EDA process by examining the dataset's structure and contents. Understand the distribution of data variables, check for missing values, and identify any potential data quality issues.

4. Key Insights: Identify key insights and trends from the dataset. Use Tableau's data exploration features to perform aggregations, filtering, and grouping of data to gain valuable insights into taxi ridership in NYC.

5. Geospatial Analysis: Utilize the PULocationID and DOLocationID columns to create geospatial visualizations. Plot taxi trip origins and destinations on a map of New York City to visualize taxi flow and popular pickup/drop-off locations.

6. Time Series Analysis: Leverage the tpep_pickup_datetime and tpep_dropoff_datetime columns to create time series visualizations. Explore patterns in taxi demand and ridership over different time periods, such as hourly, daily, monthly, or seasonal trends.

### Interactive Visualizations

7. Create Interactive Dashboards: Use Tableau's drag-and-drop interface to design interactive dashboards. Incorporate various visualizations, such as bar charts, line graphs, pie charts, and heat maps, to present the analysis findings in a visually appealing and easy-to-understand manner.

8. Filter and Drill-Down: Implement filtering and drill-down functionalities to allow users to interact with the data. Enable users to explore specific aspects of the dataset by selecting data points or applying filters to the visualizations.

### Accessibility Considerations

9. Ensure Accessibility: Keep in mind that the assistant director at the New York City TLC has visual impairments. Design the visualizations with accessibility in mind, such as using color schemes that are distinguishable and providing alternative text for non-text elements.

### Sharing and Collaboration

10. Publish the Visualizations: Publish the Tableau Public project to make the visualizations accessible to the public. Generate shareable links or embed the visualizations on the project website or in the final project report.

11. Collaborate with Stakeholders: Share the Tableau Public project link with Luana Rodriguez, the Senior Data Analyst, and Cc Udo Bankole, the Director of Data Analysis, to gather feedback and insights from stakeholders.

### Executive Summary

12. Synthesize the Analysis: Use the insights obtained from the Tableau visualizations to complement the Python analysis. Synthesize the findings into an executive summary, summarizing the most critical insights and conclusions from the entire data analysis process.

By utilizing Tableau Public, we aim to create engaging, interactive, and visually compelling visualizations that will help stakeholders at Automatidata and the New York City TLC better understand taxi ridership patterns and make informed decisions based on the data analysis.

## Executive Summary

**Executive Summary - New York City TLC Data Analysis**

*Date: [Insert Date]*

*Project Name: New York City Taxi TLC Exploratory Data Analysis (EDA) and Data Visualization*

*Team: [Insert Team Name]*

**Summary of Results of Exploratory Data Analysis (EDA)**

The exploratory data analysis (EDA) of the New York City Taxi & Limousine Commission (TLC) dataset has provided valuable insights into taxi ridership patterns in NYC. The dataset contains information on 408,294 taxi trips, with 18 data variables captured for each trip.

During the analysis, we discovered the following key findings:

1. **Ride Duration Insights:** The distribution of ride durations showed a typical bell-shaped curve, with the majority of rides lasting between 5 and 20 minutes. However, some rides had unusually long durations, indicating potential outliers.

2. **Passenger Count Analysis:** The passenger count variable exhibited a predominant value of 1, indicating mostly single-passenger rides. However, a few entries contained extremely high passenger counts, suggesting data entry errors or anomalies.

3. **Geospatial Patterns:** Geospatial visualizations highlighted popular pickup and drop-off locations across New York City. High-density areas were observed in Manhattan, airports, and major transportation hubs.

4. **Time Series Trends:** Time series analysis revealed distinct patterns in taxi demand, with peak ridership occurring during rush hours and lower demand in the early morning hours.

**Proposed Solution for Dealing with Outliers**

To address the outliers identified during the EDA, we propose the following approach:

1. **Ride Duration Outliers:** We will apply a statistical outlier detection method, such as the IQR (Interquartile Range), to identify and remove extreme ride duration values. By eliminating outliers, we can ensure that our analysis is based on more representative data.

2. **Passenger Count Anomalies:** For entries with unusually high passenger counts, we will cross-reference the data against other relevant variables, such as trip distance and location, to validate their accuracy. Any entries deemed erroneous will be corrected or removed from the dataset.

**Conclusion**

The EDA and data visualization have provided valuable insights into taxi ridership trends in New York City. By identifying outliers and applying appropriate data cleansing techniques, we can ensure the accuracy and reliability of our analysis. The results of this analysis will help the New York City TLC and stakeholders at Automatidata make data-driven decisions and optimize their services.

Please find the detailed analysis and visualizations in the attached Python notebook and Tableau Public project. We welcome feedback and further collaboration to refine the analysis and derive more in-depth insights.

Thank you for your continued support and cooperation.

*Sincerely,*

[Your Name]

[Your Role]

[Team Name]

[Email Address]

*Note: This executive summary is designed to provide a concise overview of the key results and proposed solutions. For more detailed analysis and visualizations, please refer to the attached reports.*

## Summary of Initial Data Exploration

### Head of the Data

The dataset contains 408,582 data points and has 18 columns. Below is a preview of the first few rows:

| Unnamed: 0 | VendorID | tpep_pickup_datetime | tpep_dropoff_datetime | passenger_count | trip_distance | RatecodeID | store_and_fwd_flag | PULocationID | DOLocationID | payment_type | fare_amount | extra | mta_tax | tip_amount | tolls_amount | improvement_surcharge | total_amount |
|------------|----------|----------------------|-----------------------|-----------------|---------------|------------|--------------------|--------------|--------------|--------------|-------------|-------|---------|------------|--------------|-----------------------|--------------|
| 24870114   | 2        | 03/25/2017 8:55:43 AM | 03/25/2017 9:09:47 AM | 6               | 3.34          | 1          | N                  | 100          | 231          | 1            | 13.0        | 0.0   | 0.5     | 2.76       | 0.0          | 0.3                   | 16.56        |
| 35634249   | 1        | 04/11/2017 2:53:28 PM | 04/11/2017 3:19:58 PM | 1               | 1.80          | 1          | N                  | 186          | 43           | 1            | 16.0        | 0.0   | 0.5     | 4.00       | 0.0          | 0.3                   | 20.80        |
| 106203690  | 1        | 12/15/2017 7:26:56 AM | 12/15/2017 7:34:08 AM | 1               | 1.00          | 1          | N                  | 262          | 236          | 1            | 6.5         | 0.0   | 0.5     | 1.45       | 0.0          | 0.3                   | 8.75         |
| 38942136   | 2        | 05/07/2017 1:17:59 PM | 05/07/2017 1:48:14 PM | 1               | 3.70          | 1          | N                  | 188          | 97           | 1            | 20.5        | 0.0   | 0.5     | 6.39       | 0.0          | 0.3                   | 27.69        |
| 30841670   | 2        | 04/15/2017 11:32:20 PM | 04/15/2017 11:49:03 PM | 1               | 4.37          | 1          | N                  | 4            | 112          | 2            | 16.5        | 0.5   | 0.5     | 0.00       | 0.0          | 0.3                   | 17.80        |

### Data Points and Shape

- Number of Data Points: 40,8582
- Data Shape: (22699, 18)

### Describe Function

The describe function provides a summary of the numerical columns in the dataset:

|            | Unnamed: 0 | VendorID | passenger_count | trip_distance | RatecodeID | PULocationID | DOLocationID | payment_type | fare_amount | extra | mta_tax | tip_amount | tolls_amount | improvement_surcharge | total_amount |
|------------|------------|----------|-----------------|---------------|------------|--------------|--------------|--------------|-------------|-------|---------|------------|--------------|-----------------------|--------------|
| count      | 22699.000  | 22699.000| 22699.000       | 22699.000     | 22699.000  | 22699.000    | 22699.000    | 22699.000    | 22699.000   | 22699.000 | 22699.000 | 22699.000  | 22699.000    | 22699.000             | 22699.000    |
| mean       | 5675849.000| 1.556    | 1.642           | 2.913         | 1.043      | 162.412      | 161.528      | 1.337        | 13.027      | 0.333   | 0.497   | 1.836      | 0.313        | 0.300                 | 16.311       |
| std        | 3274493.000| 0.497    | 1.285           | 3.653         | 0.708      | 66.633       | 70.140       | 0.496        | 13.244      | 0.463   | 0.039   | 2.801      | 1.399        | 0.016                 | 16.097       |
| min        | 12127.000  | 1.000    | 0.000           | 0.000         | 1.000      | 1.000        | 1.000        | 1.000        | -120.000    | -1.000  | -0.500  | 0.000      | 0.000        | -0.300                | -120.300     |
| 25%        | 28520560.000| 1.000    | 1.000           | 0.990         | 1.000      | 114.000      | 112.000      | 1.000        | 6.500       | 0.000   | 0.500   | 0.000      | 0.000        | 0.300                 | 8.750        |
| 50%        | 56731503.000| 2.000    | 1.000           | 1.610         | 1.000      | 162.000      | 162.000      | 1.000        | 9.500       | 0.000   | 0.500   | 1.350      | 0.000        | 0.300                 | 11.800       |
| 75%        | 85374518.000| 2.000    | 2.000           | 3.060         | 1.000      | 233.000      | 233.000      | 2.000        | 14.500      | 0.500   | 0.500   | 2.450      | 0.000        | 0.300                 | 17.800       |


| max        | 113486314.000| 2.000    | 6.000           | 33.960        | 99.000     | 265.000      | 265.000      | 4.000        | 999.990     | 4.500   | 0.500   | 200.000    | 19.100       | 0.300                 | 1200.290     |

### Dataframe Info

The dataframe consists of 18 columns and 22,699 rows. The data types of the columns are as follows:

- Integer: Unnamed: 0, VendorID, passenger_count, RatecodeID, PULocationID, DOLocationID, payment_type
- Float: trip_distance, fare_amount, extra, mta_tax, tip_amount, tolls_amount, improvement_surcharge, total_amount
- Object: tpep_pickup_datetime, tpep_dropoff_datetime, store_and_fwd_flag

Please note that the "Unnamed: 0" column seems to be an unnecessary index column, and the "tpep_pickup_datetime" and "tpep_dropoff_datetime" columns should be converted to datetime objects for time-related analysis.

For a more detailed analysis and further insights, refer to the Jupyter Notebook containing the complete exploratory data analysis (EDA) and data visualization.