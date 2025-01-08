# Data Analysis Report - Bike Sales 
<br />

## Table of Contents

- [Project Overview](#project-overview)
- [Preparation](#preparation)
- [Process](#process)
- [Analysis](#analysis)
- [Share](#share)
- [Recommendations](#recommendations)

---


### Project Overview

#### Objective
- To explore the data around bicycle sales.

#### Desired Outcome
- Identify factors affecting bicycle sales and provide insights and observations on these factors.
- Identify insights for marketing strategies
  
---


### Preparation

#### Data Sources
- A dataset was provided in CSV format for analysis.

#### Initial Actions

1.  Created a copy of the data for processing and transformation, ensuring integrity of original data.

2.  Identified Excel as a sufficient tool for analysis
  

---


### Process

#### Data Cleaning

- Removed duplicate entries using excels function.

- Examined data for null, missing values

#### Transformation

1.  Enabled filters on the row of field headers

2.  Checked values inside all filter fields to check and verify data and range.

3.  Used find and replace on Marital records to transform 'M' and 'S' to 'Married' and 'Single' respectively 

4.  Used find and replace on Gender records to transform 'M' and 'F' to 'Male' and 'Female' respectively 

5.  Removed decimal places from income records
  
7.  Used find and replace on 'Commute Distance' field to generate '10 Miles +' for dashboard aesthetics

8.  'Age Bracket' column created based on age records and placed into bins.
     - Young = below 31
     - Middle Age = 31-54
     - Older = 54+

     - Used nested IF statements to create the above bins:
     - =IF(L2<31,"Young",IF(L2<55,"Middle Age","Older"))

#### Visualisation

-   Created Pivot Tables and generated Charts for analysis
     - Purchase Count : Age category
     - Purchase Count : Cars Owned
     - Purchase Count : Education
     - Purchase Count : Commute Distance

-  Dashboard Creation
     - Inserted charts 
     - Added slicers to update charts when filtered on additional information:
        - Homeowner
        - Marital Status
        - Occupation
        - Gender  
      
---


### Analysis

Analysis involved exploring the data and visualisations to answer key questions

- Are there trends in Sales?

- Are there factors that affect sales significantly?

- Which groups are buying bicycles?

<br />

#### Conclusion & Findings

##### Education
- A trend in sales was identified in relation to buyers education
- Purchases increased as customer education levels increased

##### Age Groups
- Middle Aged customers were much more likely to make a purchase than any other age group
- Older people were much less likely
- Younger people were not likely at all
                
##### Car Ownership 
- The less cars a customer owned, the more likely they were to purchase a bicycle
- When a customer owned more than 2 cars, the chance of purchase dropped significantly

---


### Share

- The visualisation was shared and insights were delivered
- Recommendations were made

---


### Recommendations

- Middle age individuals showed a significantly higher interest in bicycle purchases
- Middle aged individuals were also much more likely to make a purchase
- Marketing strategies to attract more of these customers would likely be an effective way of increasing sales
- Furthermore attracting higher education levels amongst Middle-aged individuals would be a sensible target for marketing campaigns

![Screenshot 2024-12-12 104220](https://github.com/user-attachments/assets/dd51299e-7369-4e6f-9517-740ad160052f)

