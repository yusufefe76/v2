# v2
Climate-Change-and-Agricultural-Yield-Turkey
Project Idea
This project aims to explore the relationship between climate change variables, agricultural mechanization, and agricultural crop yield across Türkiye’s regions.

The hypothesis is that while higher average temperatures and lower precipitation generally lead to decreased productivity, technological inputs (specifically mechanization level) play a significant role in mitigating these effects. By analyzing both climate and machinery data, this project seeks to isolate the true impact of climate change on yield.

By combining historical meteorological data from the Turkish State Meteorological Service (MGM) with crop yield and vehicle statistics from the Turkish Statistical Institute (TÜİK), the project will identify whether changes in climate indicators are statistically correlated with agricultural performance — controlling for technological advancement.

Description of Dataset
The project will now utilize three primary datasets to ensure a robust analysis:

1. Agricultural Production Dataset (Yield Statistics)

Source: https://data.tuik.gov.tr/

Coverage: Annual crop yield (kg/decare) for key crops such as wheat, barley, corn, cotton, sunflower, etc.

Geographical Unit: Province level

Temporal Range: 2005 – 2024

Variables:

Crop type

Province

Year

Yield (kg/decare)

2. Meteorological Dataset (Climate Indicators)

Source: https://www.mgm.gov.tr/veridegerlendirme/il-ve-ilceler-istatistik.aspx

Coverage: Monthly or annual average temperature (°C) and total precipitation (mm) per province.

Temporal Range: 2005 – 2024

Variables:

Province

Average temperature

Total precipitation

Year

3. Agricultural Mechanization Dataset (New Feature)

Source: TÜİK (Motor Vehicles Statistics / Motorlu Kara Taşıtları)

Coverage: Number of tractors per province. This serves as a proxy for agricultural intensity and technological adaptation.

Temporal Range: 2005 – 2024

Variables:

Number of Tractors

Province

Year

Plan
Data Collection

Agricultural Data Sources:

TÜİK Open Data Portal → “Bitkisel Üretim İstatistikleri” (Crop Production).

TÜİK Open Data Portal → “Motorlu Kara Taşıtları” (Road Motor Vehicles) for tractor counts.

Data cleaning and transformation into time-series.

Climate Data Sources:

MGM “İl ve İlçeler İstatistikleri” for temperature and rainfall.

Aggregation from monthly → annual averages per province.

Data Analysis Approach

Exploratory Data Analysis (EDA)

Visualize yearly trends of temperature, rainfall, and crop yield.

Analyze the correlation between mechanization (tractor count) and yield growth.

Map spatial patterns of average yield vs. climate conditions.

Statistical Analysis

Compute correlation matrices between temperature, rainfall, mechanization, and yields.

Build multiple linear regression models to isolate variables:

Yield=β 
0
​	
 +β 
1
​	
 (Temperature)+β 
2
​	
 (Rainfall)+β 
3
​	
 (Tractors)+ϵ
This updated model helps determine if yield increases are due to better technology (more tractors) or climate factors.

Visualization and Presentation

Time-series line charts for yield vs. climate per crop.

Heatmaps showing correlation strength per region.

Scatter plots showing Yield vs. Tractor Count.

Tools and Technologies

Python: Main analysis language

Pandas & NumPy: Data wrangling and aggregation

Matplotlib & Seaborn: Visualization and trend analysis

Statsmodels / Scikit-learn: Regression and correlation modeling

Jupyter Notebooks: For structured and reproducible workflow

Expected Outcomes
Quantitative assessment of how temperature and precipitation variations impact crop yield.

Clear distinction between yield gains caused by technology (mechanization) vs. losses caused by climate.

Identification of crops most sensitive to heat or rainfall reduction.

Regional insights into climate vulnerability of agriculture.

Potential Challenges
Missing or inconsistent data across provinces or years.

Different measurement units or update frequencies between MGM and TÜİK.

Possible non-linear relationships requiring advanced modeling.

Data access restrictions for older years.
