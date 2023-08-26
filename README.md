
**Automatidata Project - New York City Taxi TLC Exploratory Data Analysis (EDA) and Data Visualization**

*Context: Fictional Data Scientist at Automatidata, Google Course Project*

I'm currently immersed in a fascinating project as a fictional Data Scientist at Automatidata, working on the preliminary phase of an exploratory data analysis (EDA) and data visualization initiative. Let's delve into the key aspects:

**Project Background:**

In collaboration with the New York City Taxi and Limousine Commission (TLC), my role is to embark on exploratory data analysis (EDA) and craft data visualizations utilizing Python and Tableau. The ultimate goal is to glean profound insights into the intricate patterns of taxi ridership within the dynamic landscape of New York City.

**Essential Steps and Deliverables:**

1. **Reviewing the Project Proposal:** I've meticulously reviewed the project proposal to deeply grasp its contours and aims.

2. **Inspecting and Organizing the TLC Dataset:** Armed with Python, I'm meticulously inspecting and structuring the TLC dataset, leaving no stone unturned to ensure impeccable cleanliness and impeccable structure.

3. **Email Directive from Luana Rodriguez:** An email from Luana Rodriguez, the esteemed Senior Data Analyst, has underscored the precise expectations. It calls for a Python notebook that harmoniously melds data structuring, cleansing algorithms, tantalizing matplotlib/seaborn visualizations, and visually accessible Tableau visualizations.

4. **Email Message from Udo Bankole:** Udo Bankole, the Director of Data Analysis, has reinforced the significance of an executive summary nestled alongside the Tableau visualizations and Python notebook.

5. **Python-Powered EDA:** Within the realm of Python, I'm orchestrating a comprehensive notebook that orchestrates the entire EDA symphony. This symphony comprises cleansing rituals, structured organizing, and a crescendo of visually compelling elements — including the star duets: box plots showcasing ride durations and time series masterpieces depicting temporal narratives.

6. **Tableau Artistry:** In parallel, I'm curating Tableau visualizations that seamlessly harmonize with the grand EDA narrative. These visualizations are a melange of clarity, accessibility, and the ability to resonate with both data aficionados and those navigating the territory of visual impairment.

7. **Executive Summary Crafting:** I'm meticulously distilling the crux of the analysis and findings into a refined and succinct executive summary, akin to a synopsis that captures the essence of a sprawling epic.

8. **Review and Sanctification:** Before the curtain call, I'm sharing my opus with Luana and granting Udo a backstage pass. Their insights and perspectives are invaluable before the final act unfolds.

9. **Epilogue: The Final Report:** Once the crescendo subsides, and after the analysis, visualizations, and executive summary have traversed the corridors of critique and obtained their laurels of approval, they'll convene into a grand finale — the final project report.

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
| Tolls_amount           | Total amount of all tolls paid in trip.                                                       |
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

### Executive sumary

Link: https://docs.google.com/presentation/d/1eZXLSuGKj0HByk-KT5sLlWDJeO6tITurX0ctaTG53RU/edit?usp=sharing
