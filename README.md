## AN ANALYSIS ON INSURANCE CLAIMS FOR MM INSURANCE COMPANY 


### INTRODUCTION 

MM Insurance company a top company in the vehicle insurance industry provided acomprehensive dataset for analysis. 

This dataset contains information on individual insurance policyholders, capturing various aspects of their demographics, car details, and claim history. 

Key features include age, marital status, car use (private or commercial), education level, income, car make and model, car color, and the number and amount of claims filed. The data also categorizes 
coverage zones (e.g., Rural, Urban) and includes indicators of whether children in the household drive. 

This dataset can be used to analyze patterns in claim behavior, explore the impact of demographic and vehicle characteristics on claims, and assess the relationship between household income, education, and insurance claims.

We would breakdown key findings from the dataset and give recommendations to improve future insurance claims 


### ABOUT THE DATASET 

This dataset is a synthetic collection of policyholders and other records. It includes a total of 37,542 policyholders offering insights into various demographic etc 

Below is a detailed description of the dataset: 

- Scope: Synthetic data containing 37,542 policyholders of mm insurance 

- File Type: CSV 

- Dataset: ID, birthdate, age, marital status, car use, gender, kids driving, parents, education, car make, car model, car color, car year, claim frequency, coverage zone, claim amount, household income 


### DATA CLEANING AND TRANSFORMATION 

In order to prepare our dataset for analysis, some step were included to clean the data and create calculated columns needed for analysis. Some of them are:

- Standardized all Text Format: All text format was standardized to look presentable.

- Grouped Policyholders by Age: Added an age group column to categorize policyholders age (22-30, 31-40 etc ) for better demographic analysis 

- Frequent Claimers: Added a group for frequent and non frequent claimers (where >2 is a frequent claimer) to get a better overview of claim frequency 

- Income Group: Categorizes household income into groups (50k-100k, 100k-200k etc) for better income analysis 

- Car Age: Added a column to get the age of the car ( current year - car year, where the current year is 2015) to get an overview of how old a car is for analysis 

- Car Age Group: Categorizes the age into groups (0-30, 31-40 etc) for further analysis 

- Kids Driving (Yes or No): Added a column to get household with kids driving in a yes or no format (where >= 1 is yes) for impact on claims of household with kids driving 



### ANALYSIS QUESTIONS AND INSIGHTS

#### How does claim frequency vary across different age groups, genders, and marital statuses? Are there specific demographics more likely to file frequent claims?

- Claim Frequency by Age Group: 

Younger drivers (22-29) have the highest claim frequency (>0.52), possibly due to inexperience.

The (30-39) age group has the lowest frequency (<0.51)

The (60-69) group’s low frequency may reflect limited driving, but those who do drive may still pose risks.

- Claim Frequency by Marital Status:

Claim frequency is fairly evenly distributed across marital statuses, with separated  individuals having a slightly higher share (26%).

The even distribution suggests marital status has a minimal impact on claim frequency.

Separated individuals may have higher frequency due to shared vehicles or more dependents driving.

- Claim Frequency by Gender: 

Females have a slightly higher claim frequency (0.515) than males (0.505).

The difference is minimal, suggesting gender has a limited impact on claim frequency.

Females may drive more frequently or in higher-risk areas, contributing to the slight increase.



- Is there a correlation between the level of education and the average claim amount? Do individuals with higher education levels have higher or lower claim amounts?

Bachelors and masters holders have the highest claim amount (>$50K), while PhD graduates have the lowest (<$50K).

Higher education levels correlates with higher claim amounts, with the exception of PhD holders maybe due to usage of less expensive cars 

High School graduates may have lower claim amounts due to less expensive vehicles or lower coverage levels



- How does the type of coverage zone (e.g., Rural, Urban, Highly Urban) affect claim frequency? Are people in urban areas more likely to make claims than those in rural areas?

Suburban areas have the highest claim frequency, likely due to higher traffic density and accident risks.

Highly Rural areas have the lowest claim frequency, possibly due to less traffic and lower accident rates.

Urban and highly urban areas show a slightly higher claim frequency, indicating a correlation between population density and claim likelihood.

Rural areas, while lower, still have a significant frequency, suggesting other factors like road conditions or driver behavior may contribute.



- What is the relationship between household income levels and claim amounts or frequency? Do higher income individuals file fewer claims or have lower claim amounts?

($100k-$200k) higher income level have lower claim frequency 

While ($50k-$100k) income level have higher frequency claims 

This indicates higher income individuals have fewer frequency claims 


- How does car use (Private vs. Commercial) impact the average claim amount and frequency? Are commercial car users more likely to have higher claims?

Private and commercial car use shows almost equal claim amount with very minimal difference 

This indicates the car type has no effect on the claim amount 


- Does having kids who drive influence claim frequency or amount? Are there significant differences in claim behavior between households with and without kids driving?

Claim frequency of (0.512) where kids are not driving vs frequency of (0.506) where kids are driving 

The indicates a significant difference in households with kids driving and not driving and households where kids are driving have minimal claim frequency compared to households without kids driving 

Indicating kids driving have minimal impact on claims frequency 


- Which car makes (e.g., Acura, Nissan, Ford) have the highest and lowest average claim amounts? Are certain brands associated with higher insurance claims?

Hillman vehicles have the highest average claim amount ($54K), while Rambler vehicles have the lowest ($16K).

Hillman vehicles may be more expensive to repair or replace, leading to higher claim amounts.

Rambler vehicles may be older or less costly, resulting in lower claim amounts.


- How does the car’s model year relate to claim amount and frequency? Are older cars associated with more frequent claims or higher claim amounts?

Claim frequency fluctuates over the years, with notable peaks in 1954, 1970, and 1986

Recent years (1990-2010) show a decline in frequency.

Peaks may correspond to economic or social factors (e.g., increased car ownership, road congestion).

The decline in recent years could be due to improved vehicle safety features or stricter regulations.


- How does household income relate to the chosen coverage zone? Are higher income individuals more likely to be in highly urban areas, and does this affect their claim amount or frequency?

<$50k income earners are found in highly rural areas with very high claim amounts of over ($50k)

Also income level of $200k - $500k living in highly rural areas also have high claim amounts, this maybe b due to bad roads in this areas and probably theft also 

All income categories earners living in the highly urban areas have the lowest claim amount 



STRATEGIC RECOMMENDATIONS 

Demographic Targeted Pricing
Raise premiums for young drivers (22-29) due to high claim frequency (>0.52); offer telematics discounts for safe driving.

Lower premiums for PhD holders and 30-39 age group with low claim frequency/amounts (<$50K, <0.51).

Slightly increase rates for separated individuals (26% claim share) due to shared vehicle risks.


Zone-Based Risk Management

Increase premiums in suburban areas (highest claim frequency) and urban zones; lower rates in highly rural areas but add theft/road hazard coverage for high claim amounts (>$50K).

Use telematics in urban/suburban areas to monitor driving and reduce claims.


Income and Education Adjustments

Offer discounts for higher income ($100k-$200k) customers with lower claim frequency; promote usage based insurance for middle income ($50k-$100k) with higher frequency.

Raise premiums for bachelor’s/master’s holders (claims >$50K); maintain moderate rates for high school graduates.


Vehicle Specific Strategies

Increase premiums for Hillman vehicles ($54K claims); discount Rambler vehicles ($16K claims).

Surcharge older models (1954, 1970, 1986) with high claim frequency; discount newer models (1990-2010) with safety features.


Family and Commercial Policies

Offer family discounts for households with teen drivers (lower frequency: 0.506) enrolled in safe driving programs.

Maintain consistent pricing for private/commercial vehicles; monitor commercial mileage via telematics.


Marketing and Innovation

Target higher-income, PhD, and rural customers with tailored coverage and safety focused marketing.

Expand telematics and predictive analytics to personalize pricing and reduce claim frequency.

Partner with automakers for safety feature discounts and local governments to improve rural roads.


Compliance and Ethics

Ensure pricing complies with anti discrimination laws; audit models for bias.

Protect telematics data and communicate privacy policies clearly.



CONCLUSION 

Optimize pricing for high risk groups (young drivers, suburban residents) and low-risk segments (PhD holders, higher income) using telematics and analytics. Tailor coverage for rural theft/road risks and urban collision needs. Promote safe driving and newer vehicles through discounts and partnerships to reduce claims while ensuring fair, compliant practices.
