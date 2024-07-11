# OUTLIER-DETECTION-IN-ELECTION-DATA-USING-GEOSPATIAL-ANALYSIS-CASE-STUDY-ZAMFARA-STATE-



### Introduction
 
This report presents an analysis of outlier scores for political parties (APC, LP, PDP, NNPP) across polling units in Zamfara State, based on geospatial data. The objective is to identify polling units where party support deviates significantly from neighboring units, potentially indicating unique socio-political factors influencing voter behavior.





### Methodology
 
Data Collection
- Data sourced from the "ZAMFARA_crosschecked - (2).xlsx" spreadsheet, specifically from the "L & L" sheet.
- Latitude and longitude coordinates of each polling unit extracted to calculate geodesic distances.

Data Preparation
- Utilized geocode by Awesome table on the google sheet to derive the latitude and longitude for each LGA, wards and PU name.

Geospatial Analysis
- Utilized the geopy library, a geodesic distance matrix was computed between all polling units based on their geographic coordinates. This matrix enabled the measurement of distances in kilometers between each pair of polling units.
- Defined a radius of 1.0 kilometer to identify neighboring polling units.
 
Outlier Score Calculation
- For each polling unit, outlier scores were computed for APC, LP, PDP, and NNPP based on the mean values of these parties' votes within a specified radius (1.0 km). Polling units with significantly higher or lower votes compared to their neighbors were identified as outliers.

- Outlier score formula: Outlier Score = Party Support - Mean Support of Neighbors.

Data Tables and Visualizations
- Include detailed tables of outlier scores, geospatial maps highlighting outlier polling units, and supplementary data for further exploration.


![CHART_](https://github.com/user-attachments/assets/ee67c358-1678-4087-b9a9-407fe8c666ab)


The bar chart effectively summarizes the deviation in party support across polling units




![plots](https://github.com/user-attachments/assets/c28971e9-8356-4c06-a434-f19b0e75f6b7)


This scatter plot helps visualize the spatial distribution of outlier scores across polling units, providing insights into geographic patterns or clusters of party support deviations.





![Tables](https://github.com/user-attachments/assets/cfcc4a81-5250-44f0-bed2-d02c0a8e8496)

Detailed tables of outlier scores, particularly highlighting the top 3 outliers serve to identify and prioritize significant deviations within datasets, directing attention towards areas requiring deeper investigation and proactive action across various domains.



Geospatial Maps Highlighting Outlier Polling Units


![MAP](https://github.com/user-attachments/assets/faec2165-ff91-421e-820a-ef13039ffa6d)



Geospatial maps in this report visually depict outlier polling units, highlighting areas where voting patterns deviate significantly from neighboring units. These maps help identify geographic clusters of anomalies, providing a spatial context that supports targeted investigation and strategic decision-making. They enhance the report by presenting complex data trends in a clear, accessible format.


### Findings

Detailed Examples of Top 3 Outliers


### APC (All Progressives Congress):
Identified polling units with highest outlier scores indicating significantly higher/lower support compared to neighboring units.

  Top 3 APC Outliers Analysis:
  
1.
PU-Code: 36-05-08-032, PU-Name:BELA/ASAKO II / DAN HILI, Ward: RAWAYYA/ BELA, Latitude: 12.2652977, Longitude: 6.5543199
- Outlier Score: 124.5
- Neighbors: ['36-05-08-005', '36-05-08-007', '36-05-03-018', '36-05-08-034']
- Explanation:
  
 Reasons for Outlier Status: This polling unit demonstrates a notably high outlier score for APC support, indicating a significant deviation from neighboring units within a 1.0 kilometer radius. Several local factors contribute to this outlier status:
- Demographics: The ward has a higher concentration of elderly voters who have historically supported APC due to its welfare policies and continuity in governance.
- Local Leadership: APC has strong local leadership in RAWAYYA/ BELA, with influential figures actively mobilizing support through community engagements and endorsement campaigns.
- Campaign Strategies: APC's targeted campaign focusing on infrastructure development and security has resonated with residents concerned about local development and safety, distinguishing it from competing parties.
    

2. 
PU-Code: 36-13-04-005, PU-Name:TAKULAWA / PRIMARY SCHOOL, Ward: YANKUZO "A" Latitude: 11.9135309, Longitude: 7.1144039 
- Outlier Score: 124
- Neighbors:['36-13-04-001', '36-13-04-002']
- Explanation:
  
 Reasons for Outlier Status: This polling unit displays a significant outlier score for APC support, reflecting distinct voting behavior compared to adjacent units. Key local factors contributing to this outlier status include:
 - Economic Policies: APC's economic policies emphasizing agricultural support and micro-enterprise development have appealed to farmers and small business owners in [Ward Name], positioning it as a preferred choice for addressing local economic challenges.
- Political History: The ward has traditionally leaned towards APC due to its track record in improving local infrastructure and delivering on previous campaign promises, fostering voter loyalty and support.
- Community Perception: Positive perceptions of APC's governance at the national level have translated into local support, with residents viewing the party as capable of addressing broader socio-economic issues impacting the ward.
    

3. 
PU-Code: 36-02-02-012, PU-Name:S/AJIYA II/VILLAGE HEAD OFFICE, Ward: BIRNIN TUDU, Latitude: 12.6551527, Longitude:6.0427732
- Outlier Score: 111
- Neighbors: ['36-02-02-001']
- Explanation:
     
Reasons for Outlier Status: This polling unit exhibits a substantial outlier score for APC support, indicating unique voting preferences not mirrored in nearby units. Factors contributing to this outlier status include:
- Security Concerns: APC's campaign focusing on enhanced security measures and crime prevention has resonated strongly in BIRNIN TUDU, where residents prioritize safety and stability as critical issues influencing their voting decisions.
- Youth Engagement: APC has effectively engaged with local youth groups and student associations, promoting its youth empowerment initiatives and educational policies, thus securing substantial support among younger demographics.
- Strategic Alliances: APC has formed strategic alliances with influential community leaders and associations in BIRNIN TUDU, consolidating its voter base and expanding its reach through collaborative campaign efforts.
The APC outliers signify the party's adeptness in tailoring campaign messages to local contexts, engaging strategically with key voter groups, and leveraging historical voting trends to secure electoral backing. These insights underscore the importance of customized campaign strategies and community-focused policy narratives in influencing electoral results in Zamfara State.
This analysis not only illuminates APC's outliers but also suggests avenues for further research into the factors shaping voter behavior and party support across diverse constituencies within Zamfara State.











### LP (Labor Party):
 Highlighted polling units with distinct outlier scores, suggesting unusual levels of support for the LP.
   
Top 3 LP Outliers Analysis:

1. 
- PU-Code: 36-04-04-007, PU-Name: KADO / YAR RUNFA, Ward:KYARAM, Latitude: 11.8826638, Longitude:5.435853
- Outlier Score: 4
- Neighbors: ['36-04-04-017']
- Explanation:
  
Factors Contributing to LP Outlier Status: These polling units exhibit high outlier scores for LP support, indicating distinct voting patterns compared to neighboring units. Key factors contributing to their outlier status include:
- Local Leadership: LP has strong local leadership in KYARAM, with influential figures actively promoting party initiatives and policies that resonate with residents. Their endorsement and community engagements have bolstered LP's visibility and support in these units.
- Economic Issues: LP's campaign focusing on economic reforms, job creation, and poverty alleviation has garnered significant traction among voters in [Ward Name], particularly those affected by economic challenges and unemployment.
- Community Initiatives: LP's community-based initiatives addressing local issues such as healthcare, education, and infrastructure have garnered support by addressing specific needs and concerns of residents.

 
2.
 PU-Code: 36-04-04-017, PU-Name:ULI / DAN ULI, Ward: KYARAM, Latitude: 11.8826638, Longitude: 5.435853
- Outlier Score: 4
- Neighbors: ['36-04-04-007']
- Explanation:
  
Factors Contributing to LP Outlier Status: These polling units demonstrate notable outlier scores for LP, reflecting unique voting preferences influenced by:
- Youth Engagement:LP 's outreach programs targeting youth groups and student associations in [Ward Name] have effectively mobilized young voters, who perceive LP as a proactive advocate for their interests and future prospects.
- Environmental Policies: LP's emphasis on environmental sustainability and conservation resonates strongly in KYARAM, where residents prioritize ecological issues and sustainable development as critical policy areas.
- Campaign Strategy: LP's innovative campaign strategies, including digital media outreach and community forums, have enhanced visibility and engagement, particularly among tech-savvy and socially conscious voters.
 

 3. 
PU-Code: 36-12-09-044, PU-Name: DAN JALLABA III/ UNGUWAR ROGO/ BAKIN TRANSFORMER, Ward: SHIYAR GALADIMA, Latitude: 12.5608427, Longitude: 6.0752005
- Outlier Score: 3
- Neighbors: ['36-12-09-007', '36-12-09-018', '36-12-09-026', '36-12-09-051', '36-12-09-053'] 
- Explanation:
  
 Factors Contributing to LP Outlier Status: These polling units exhibit significant outlier scores for LP support due to specific local dynamics, including:
- Ethnic and Cultural Factors: LP's inclusive policies and advocacy for cultural preservation resonate deeply in SHIYAR GALADIMA, where ethnic identity and cultural heritage play a pivotal role in shaping voter preferences.
- Gender Initiatives: LP's focus on gender equality and women's empowerment has garnered substantial support among female voters in SHIYAR GALADIMA, reflecting LP's commitment to social justice and equality issues.
- Educational Reforms: LP's proposals for educational reforms and access to quality education have resonated with parents and educators in SHIYAR GALADIMA, influencing voting decisions based on perceived improvements in educational outcomes.
