Back to [Data Analytics Projects](<../../README.md>)

# **Client Risk Analysis: 360° Overview Dashboard**

**Goal:** Yearly review of credit risk per client.<br>
**Function:** 360° Overview Dashboard provides all information relevant to the client's credit risk on one page, facilitating faster decision making.<br>
**Tools used:** MS Power BI<br>



## Background

This company is in the business of billing and collections on behalf of a network of stone quarries. Clients load up on the materials at the distribution sites and pay monthly upon receipt of an invoice. The company wants to follow and manage credit risk at the client level. 

Client Risk Analysis: 360° Overview Dashboard\
![](<Client%20risk%20360%20overview.jpg>)

## Dashboard Elements

### Client Selectors *(top right page)*

The first slicer from the top allows the user to view information based on the client number.

The second slicer allows the user to review clients based on the importance of their business to the company. Clients are ranked from 1 to X from the highest to lowest turnover in the prior year. 

*Utility:* Gain a comprehensive overview of all client-related metrics at a glance. The second slicer ensures that evaluation of the most important clients is prioritised.

### Credit Ceiling *(center left page)*

Historic time series comparison of monthly <span style="color:green">outstanding balances (green columns)</span> to <span style="color:blue">monthly turnover (blue columns)</span> and currently approved <span style="color:red">credit ceiling (red line)</span>. When the outstanding balance exceeds the current approved credit ceiling, SAP R/3 BW InfoCube includes this in the daily report, and the client is invited to pay the outstanding balance before shopping for more materials.

*Utility:* Aids the decision to increase the approved credit ceiling or to release some of the collateral and decrease it.        

### Payment Behaviour *(bottom left page)*
 
Shows payment delay of every invoice. <span style="color:green">The green horizontal line</span> marks 15-day threshhold of early payment discount, <span style="color:red">the red horizontal line</span> marks invoice due date. 

*Utility:* Helps evaluate client's payment behaviour and it's evolution over time. 

### Late Payment Interest *(center right page)*

Shows previously invoiced late payment interest and whether it was <span style="color:green">paid</span> or <span style="color:orange">not paid</span>.

*Utility:* Decision aid

### Credit Ceiling and Risk Rating Change History *(bottom right page)*

Shows previous changes in credit ceiling and risk rating. 

*Utility:* Memory aid for previous decisions

## Dashboard Improvement Opportunities

- Client Risk Scoring: Apply statistical methods to calculate client risk scores based on historical data, incorporating key risk indicators.
- Dynamic Risk Updates: Leverage machine learning models to dynamically update risk scores by identifying evolving patterns and trends.
- Credit Default Prediction: Use logistic regression to classify clients as likely or unlikely to default on their payments, enabling proactive risk management.



Back to [Data Analytics Projects](<../../README.md>)