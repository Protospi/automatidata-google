## Automatidata Project - New York City Taxi TLC Exploratory Data Analysis (EDA) and Data Visualization

<p align="center">
  <img src="cabs.jpeg" alt="New Yor City Cab">
</p>

*Context: Fictional Data Scientist at Automatidata, Google Course Project*

**Project Background:**

In collaboration with the New York City Taxi and Limousine Commission (TLC), my role is to embark on exploratory data analysis (EDA) and craft data visualizations utilizing Python and Tableau. The ultimate goal is to glean profound insights into the intricate patterns of taxi ridership within the dynamic landscape of New York City.

**Essential Steps and Deliverables:**

- **Inspecting and Organizing the TLC Dataset:** Armed with Python, I'm meticulously inspecting and structuring the TLC dataset, leaving no stone unturned to ensure impeccable cleanliness and impeccable structure.

- **Email Directive from Luana Rodriguez:** An email from Luana Rodriguez, the esteemed Senior Data Analyst, has underscored the precise expectations. It calls for a Python notebook that harmoniously melds data structuring, cleansing algorithms, tantalizing matplotlib/seaborn visualizations, and visually accessible Tableau visualizations.

- **Email Message from Udo Bankole:** Udo Bankole, the Director of Data Analysis, has reinforced the significance of an executive summary nestled alongside the Tableau visualizations and Python notebook.

- **Python-Powered EDA:** Within the realm of Python, I'm orchestrating a comprehensive notebook that orchestrates the entire EDA symphony. This symphony comprises cleansing rituals, structured organizing, and a crescendo of visually compelling elements — including the star duets: box plots showcasing ride durations and time series masterpieces depicting temporal narratives.

- **Tableau Artistry:** In parallel, I'm curating Tableau visualizations that seamlessly harmonize with the grand EDA narrative. These visualizations are a melange of clarity, accessibility, and the ability to resonate with both data aficionados and those navigating the territory of visual impairment.

- **Executive Summary Crafting:** I'm meticulously distilling the crux of the analysis and findings into a refined and succinct executive summary, akin to a synopsis that captures the essence of a sprawling epic.

- **Review and Sanctification:** Before the curtain call, I'm sharing my opus with Luana and granting Udo a backstage pass. Their insights and perspectives are invaluable before the final act unfolds.

- **Epilogue: The Final Report:** Once the crescendo subsides, and after the analysis, visualizations, and executive summary have traversed the corridors of critique and obtained their laurels of approval, they'll convene into a grand finale — the final project report.

**Summation of Approach and Discovery:**

- The PACE framework, a virtuoso performance in Planning, Analysis, Construct, and Execution, has been our guiding star.
- The dataset has been sanctified through data quality assessments and meticulous cleaning rituals.
- A symphony of descriptive statistics and mesmerizing visualizations has illuminated ride durations, passenger counts, geospatial dynamics, and temporal crescendos.
- Outliers, akin to intriguing soloists in this grand concerto, have been handled with statistical finesse.
- Enter Tableau Public, our visual maestro, leading the charge with interactive visualizations that beckon exploration. Behold the visual symphony [here](https://public.tableau.com/app/profile/pedro.loes/viz/TLCTaxiData/DistancexAmount).
- The [Executive Summary](https://docs.google.com/presentation/d/1eZXLSuGKj0HByk-KT5sLlWDJeO6tITurX0ctaTG53RU/edit?usp=sharing) is akin to the opening notes of an opera, setting the stage for the drama to unfold.

For a more elaborate exploration and a deeper plunge into insights, kindly refer to the attached Jupyter Notebook and partake in the visual voyage provided by the Tableau Public link.

## Data Dictionary

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
| Tolls_amount          

 | Total amount of all tolls paid in trip.                                                       |
| Total_amount           | The total amount charged to passengers. Does not include cash tips.                           |

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

For a more detailed analysis and further insights, refer to the Jupyter Notebook containing the complete exploratory data analysis (EDA) and data visualization.

### Tableau Public

Link: https://public.tableau.com/app/profile/pedro.loes/viz/TLCTaxiData/DistancexAmount

### Executive Summary

Link: https://docs.google.com/presentation/d/1eZXLSuGKj0HByk-KT5sLlWDJeO6tITurX0ctaTG53RU/edit?usp=sharing

# Jupyter Notebook Hypothesis Test

In this section of the larger project, we delve into a focused exploration using a Jupyter Notebook to conduct a hypothesis test. The main objective of this endeavor is to analyze the relationship between payment methods and fare amounts in the context of taxi services. The project follows a structured approach, encompassing data preparation, hypothesis testing, and insightful communication of findings.

## Part 1: Imports and Data Loading

### Plan Stage

In the planning phase of our hypothesis test, we set the foundation for the analysis by defining our research question and formulating the corresponding null and alternative hypotheses.

### Research Question

Our research question is: **Does the choice of payment method influence the fare amount for taxi rides?**

### Hypotheses Formulation

In hypothesis testing, we set up two hypotheses: the null hypothesis (H0) and the alternative hypothesis (H1). These hypotheses represent competing claims about our research question.

**Null Hypothesis (H0):** The choice of payment method does not have a significant impact on the fare amount for taxi rides.

**Alternative Hypothesis (H1):** The choice of payment method does have a significant impact on the fare amount for taxi rides.

By formulating these hypotheses at the outset, we establish a clear direction for our analysis. The null hypothesis represents the absence of an effect, while the alternative hypothesis suggests the presence of an effect.

As we proceed with the analysis, we will gather evidence from the data to decide whether we have enough evidence to reject the null hypothesis in favor of the alternative hypothesis.

## Part 2: Conduct EDA and Hypothesis Testing

### Analyze and Construct Stage

As we move into the "Analyze and Construct" stage of our project, we leverage descriptive statistics for Exploratory Data Analysis (EDA). Descriptive statistics serve as valuable tools to unravel insights hidden within the dataset. Let's explore how computing descriptive statistics enhances our understanding of the data in this stage of analysis.

**Exploring Data with Descriptive Statistics**

Descriptive statistics provide a concise summary of key characteristics of the dataset. They include measures such as mean, median, standard deviation, minimum, maximum, and quartiles. In the context of our hypothesis test, computing descriptive statistics helps us in the following ways:

1. **Central Tendency:** Calculating the mean and median of fare amounts based on different payment methods gives us a sense of the typical fare values. This helps us understand the average fare amounts associated with each payment type.

2. **Variability:** Standard deviation reveals how much the fare amounts deviate from the mean. Higher standard deviation might indicate greater variability in fare amounts for a particular payment method.

3. **Distribution:** Creating histograms or density plots of fare amounts for different payment methods allows us to visualize their distributions. This can uncover patterns or anomalies.

4. **Comparison:** Comparing descriptive statistics between payment methods allows us to identify potential differences. For instance, comparing means could hint at whether one payment method tends to yield higher fare amounts.

By employing descriptive statistics, we construct a solid foundation for our hypothesis test. These statistics offer a preliminary understanding of the dataset's characteristics, helping us recognize trends, disparities, and potential outliers. This knowledge guides our subsequent hypothesis testing by providing context and initial evidence for or against our research question.

### Hypothesis Test

### Task 3. Hypothesis testing

$H_0$: There is no difference in the average fare amount between customers who use credit cards and customers who use cash.

$H_A$: There is a difference in the average fare amount between customers who use credit cards and customers who use cash.

The hypothesis test comparing average fare amounts between credit and cash payments yields the following results:

1. **Test Statistic:** -6.866800855655372
2. **P-value:** 6

.797387473030518e-12 (approximately 0.0000000000068)

Based on these results:

- The test statistic of -6.866800855655372 indicates how many standard deviations the sample mean of the difference between credit and cash payments' fare amounts is from the expected mean difference under the null hypothesis.

- The p-value of 6.797387473030518e-12 is extremely small, almost equal to zero. This indicates strong evidence against the null hypothesis that there is no difference in average fare amounts between credit and cash payments considering a significance level of 0.05.

Given the very low p-value, we have reason to reject the null hypothesis. This suggests that there is a statistically significant difference in average fare amounts between credit and cash payments. In other words, the evidence suggests that payment method does influence the fare amount, and the difference in average fare amounts is unlikely to have occurred by chance.

The p-value is approx 0, so we reject the null hypothesis that there's no difference in fare amount between the payment types credit card and cash. In other words, there's statistical evidence with a significance level of 0.05 that the mean of fare amount of credit card payments is different from the mean of cash payments.

These results support the initial intuition that there might be a relationship between payment method and fare amounts, as indicated by the analysis and the previous findings.