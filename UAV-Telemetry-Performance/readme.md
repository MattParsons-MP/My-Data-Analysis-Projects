# Data Analysis Report on UAV RF Telemetry Performance 
<br />

## Table of Contents

- [Project Overview](#project-overview)
- [Preparation](#preparation)
- [Process](#process)
- [Analysis](#analysis)
- [Share](#share)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

---


### Project Overview

#### Objective
- To analyse and improve telemetry performance between an airborne craft and its ground control station.

#### Key Problem
- Telemetry relies on a stable radio link to send critical flight data to the ground station.
- Signal inconsistencies reduce mission effectiveness by limiting range and compromising the pilot's ability to receive essential flight information.

#### Desired Outcome
- Identify and address factors affecting telemetry performance, aiming to enhance range and data integrity under diverse flight conditions.
  
---


### Preparation

#### Data Sources
- A blackbox log of flight data provided in a CSV format for analysis.

- Stakeholder-provided dataset with permission to publish, except for GPS positional data.

#### Initial Actions

1.  Created a copy of the data for processing and transformation, ensuring integrity of original data.

2.  Data Transformation requirements - Identified software and formats necessary for cleaning, transformation and geospatial visualisations.

3.  Identified methods to obscure GPS data prior to publishing.

---


### Process

#### Data Cleaning

- Removed irrelevant columns to focus on 13 key fields, including Duration, TQly (link quality), TRSS (signal strength), GPS coordinates, and Pitch/Roll angles.

- Examined data for null, missing and duplicate values

#### Transformation

1.  Added Row numbers to create progress fields

2.  Segmented flight data to calculate outbound and return journey progress.

3.  Converted various units of measurement into local format

4.  Handled unusable time data and created duration field

5.  Split GPS data into seperate fields to utilise Geospatial mapping visualisaton

---


### Analysis

Analysis involved exploring the data and visualisations to answer key questions

- Are there trends in signal strength or Loss?

- Where is signal Strongest an weakest?

- Are there any standout observations?

<br />

#### Conclusion & Findings

##### Aircraft Turns 
- Detected significant signal strength drops during aircraft turns.

##### Flight Phases 
- Outbound leg flown at a Lower, inconsistent flight profile correlated with poor signal consistency.
- Return leg flown at Higher, consistent flight profile improved RF performance hinting at the altitude and flight profile's role in signal stability.
                
##### Power Consumption 
- Lower current draw during descent phases may have contributed to better receiver performance due to reduced system noise, interference and power drain.

---


### Share

- Using geospatial visualisation software, the flight data was mapped to overlay telemetry strength and all other telemetry data.
- The visualisation was presented to stakeholders to illustrate key findings, showing how flight profile and altitude directly impacted RF performance.

- The importance of antenna alignment was emphasised along with the potential for improving system design to mitigate identified issues.

##### Feedback 
- The visualisation clarified the challenges with antenna alignment and the impact of inconsistent flight paths on signal strength.
- Stakeholders agreed on the need for hardware and operational changes to improve telemetry reliability.

![1725714781196](https://github.com/user-attachments/assets/06717ca5-5e6c-444f-9839-b14c349e730e)



---


### Recommendations

#### Operational

- Implement operational changes to improve flight profile consistency

- Explore technology utilising multiple antennas, aligned for differing phases of flight.

- Explore automated antenna alignment systems for aircraft

- Implement a dynamic ground antenna capable of aligning with aircraft flight angles.

- Investigate if reduced power consumption during descent correlates with better RF performance and adapt procedures accordingly

---


### Conclusion

- The visualisation and analysis highlighted the critical role of flight profile and antenna alignment in telemetry performance. 

- Maintaining consistent altitudes and improving antenna systems are key steps toward enhancing mission reliability. 

- Proposed solutions range from cost-effective diversity antenna systems to advanced dynamic antenna systems. 

- Further testing is recommended to validate these recommendations under varied operational conditions.
