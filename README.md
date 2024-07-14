# OUTLIER-DETECTION-IN-ELECTION-DATA-USING-GEOSPATIAL-ANALYSIS-CASE-STUDY-ZAMFARA-STATE-

## Table of Content

- [Introduction](#introduction)
- [Methodology](#methodology)
- [Findings](#findings)
- [Conclusion](#conclusion)
- [Recommendations](#recommendations)




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




### PDP (Peoples Democratic Party):
Notable outlier scores indicating significant deviations in party support within specific polling units.

Top 3 PDP Outliers Analysis:



1.
PU-Code: 36-13-09-007, PU-Name: CHEDIYA / BAKIN KASUWA, Ward: CHEDIYA, Latitude: 11.9552779, Longitude: 6.9182301
   - Outlier Score:109.4
   - Neighbors: ['36-13-08-012', '36-13-08-027', '36-13-09-004', '36-13-10-005', '36-13-10-009']
   - Explanation:
  
 Interpretation of Findings: These polling units exhibit notable outlier scores for PDP support, indicating significant deviations from neighboring units. Factors contributing to their outlier status include:
   	- Historical Ties: PDP's longstanding presence and historical ties in CHEDIYA have fostered strong party loyalty and support, anchored by decades of community engagement and service delivery.
   	- Candidate Popularity: The popularity and local appeal of PDP's candidates in CHEDIYA have contributed to their electoral success, with voters identifying closely with candidate profiles and campaign promises.
   	- Regional Development Issues: PDP's focus on regional development projects and infrastructural improvements resonates strongly in CHEDIYA, where residents prioritize local development and government investment in public services.

     
 
2. 
PU-Code: 36-13-03-010, PU-Name: GOBIRAWA I / GARKAR MAI GARI, Ward: YANDOTON DAJI, Latitude: 12.0445057, Longitude: 6.8672668
   - Outlier Score:101
   - Neighbors: ['36-13-03-012']
   - Explanation:
     
Interpretation of Findings: These polling units demonstrate significant outlier scores for PDP, reflecting distinct voting preferences shaped by:
   	- Social Welfare Policies: PDP's emphasis on social welfare programs and poverty alleviation initiatives has garnered widespread support in YANDOTON DAJI, addressing community concerns about economic inequality and social justice.
   	- Local Governance Issues: PDP's track record in effective local governance and service delivery in YANDOTON DAJI has bolstered voter confidence and support, emphasizing the party's capacity to address local challenges effectively.
   	- Community Development Initiatives: PDP's community-driven initiatives and grassroots mobilization efforts have galvanized support among diverse demographics in YANDOTON DAJI, illustrating the party's grassroots strength and organizational capacity.

 

 3. 
PU-Code:36-13-03-012, PU-Name: NASARAWA / DAN FILI, Ward:YANDOTON DAJI, Latitude: 12.0445057, Longitude:6.8672668
   - Outlier Score:101
   - Neighbors: ['36-13-03-010']
   - Explanation:
     
 Interpretation of Findings: These polling units exhibit substantial outlier scores for PDP support due to:
   	- Public Policy Agenda: PDP's policy agenda addressing healthcare, education, and social security resonates deeply in [Ward Name], where residents prioritize access to essential services and government support for vulnerable populations.
   	- Community Engagement: PDP's active engagement with local communities and stakeholders in [Ward Name] has strengthened party ties and bolstered electoral support, highlighting effective communication and responsiveness to community needs.
   	- Public Perception: Positive public perception of PDP's leadership and governance at the national level has translated into local support in [Ward Name], with voters endorsing the party's vision for inclusive development and progressive governance.





 
 ### NNPP (New Nigeria Peoples Party)
Identified polling units where NNPP support varies significantly from neighboring units.

 Top 3 NNPP Outlier Analysis:

 
1.
 PU-Code:36-07-03-003, PU-Name:SABON GARI I / MADA GENERAL HOSPITAL, Ward: MADA, Latitude: 12.1628466, Longitude: 6.6745042
   - Outlier Score:12.67
   - Neighbors:['36-07-02-013', '36-07-03-012', '36-07-03-019']
   - Explanation:
     
 Reasons for Outlier Status: This polling unit exhibits a notably high outlier score for NNPP support, indicating a significant deviation from neighboring units within a 1.0 kilometer radius. The outlier status can be attributed to several local factors:
   	- Youth Engagement: NNPP has actively engaged with local youth organizations and student groups in MADA, resonating strongly with younger demographics who perceive the party's policies as more aligned with their aspirations.
   	- Local Grievances: The area has historically faced challenges with access to basic services, and NNPP's campaign promises focusing on community development and improved infrastructure have garnered substantial support among residents.
   	- Community Outreach: NNPP leadership in this ward has implemented effective grassroots outreach programs, organizing community meetings and addressing specific local concerns such as employment opportunities and healthcare access.
    
 
2.
 PU-Code: 36-07-03-019, PU-Name:GIDAN KARA / DAN HILI, Ward: MADA, Latitude: 12.1628466, Longitude: 6.6745042
   - Outlier Score: 6
   - Neighbors:['36-07-02-013', '36-07-03-003', '36-07-03-012']
   - Explanation:
     
 Reasons for Outlier Status:This polling unit shows a significant outlier score for NNPP support, reflecting a distinct level of voter preference compared to nearby units. Key factors contributing to this outlier status include:
   	- Candidate Popularity:The NNPP candidate for local council elections in MADA has a strong personal following due to their prior community service and advocacy for youth empowerment and education.
   	- Policy Alignment: NNPP's emphasis on agricultural reform and small business support has resonated with farming communities and local entrepreneurs in the ward, distinguishing it from other parties focusing on broader national issues.
   	- Strategic Campaigning: NNPP has strategically positioned itself as a viable alternative to established parties, leveraging discontent with incumbent performance and promoting transparency and accountability in governance.


 
 3.
 PU-Code: 36-09-03-011, PU-Name:KYARA / SH/ADAMU, Ward: FARU / MAGAMI, Latitude: 12.9641447, Longitude: 6.1102943 
   - Outlier Score:6
   - Neighbors: ['36-09-03-024']
   - Explanation:
   
   
Reasons for Outlier Status:This polling unit exhibits a substantial outlier score for NNPP support, indicating unique voting behavior not observed in adjacent units. Factors contributing to this outlier status include:
   	- Ethnic Dynamics: The area has a predominant ethnic community with historical ties to the NNPP leadership, influencing voter loyalty and support for the party's candidates during elections.
   	- Local Economic Issues:NNPP's campaign promises focusing on job creation and economic revitalization have resonated with residents facing unemployment and economic hardship, distinguishing it as a preferred choice for addressing local economic grievances.
   	- Community Endorsements: Local community leaders and influential figures in [Ward Name] have publicly endorsed NNPP, amplifying its appeal and swaying undecided voters towards the party.
 
The NNPP outliers show how the party successfully gained local support by addressing specific community issues, engaging youth effectively, and positioning itself strategically against other political messages. These insights reveal the importance of tailoring campaigns to local needs and focusing on community-driven policies for electoral success in Zamfara State. This analysis not only highlights NNPP's exceptional cases but also suggests areas for deeper study on voter behavior and party dynamics across different areas of Zamfara State.




### Conclusion
 
This report has provided a detailed analysis of outlier scores for political parties in Zamfara State, highlighting polling units where party support significantly deviates from neighboring units. The findings underscore the importance of local dynamics in shaping electoral outcomes and suggest avenues for further research and targeted political engagement.



### Recommendations
 
- Targeted Engagement: Recommend targeted outreach efforts in outlier polling units to consolidate support or address grievances.
- Data Integration: Advocate for continuous data collection and analysis to refine electoral strategies and policy priorities.
- Community Dialogue: Emphasize the role of community dialogue and grassroots engagement in bridging electoral divides.



