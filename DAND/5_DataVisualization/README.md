<img width="90%" border="30" src="https://user-images.githubusercontent.com/13763933/51613814-e1f3a380-1f56-11e9-8d60-9a147acc23bd.png"/>
<br>

# Data Visualization
This project was completed as part of the course requirements of Udacity's [Data Analyst Nanodegree](https://www.udacity.com/course/data-analyst-nanodegree--nd002) certification.

## Overview
This project has two parts that demonstrate the importance and value of data visualization techniques 
in the data analysis process. In the first part, you will use Python visualization libraries to systematically
explore a selected dataset, starting from plots of single variables and building up to plots of multiple 
variables. 

In the second part, you will produce a short presentation that illustrates interesting properties, 
trends, and relationships that you discovered in your selected dataset. 
The primary method of conveying your findings will be through transforming your exploratory 
visualizations from the first part into polished, explanatory visualizations.

## Technologies Used
- Python 
- Libraries: pandas, numpy, matplotlib, seaborn, plotly
- Jupyter Notebook

## Key Findings
- From plotly, most big airports are locoated on the East coast. Also most delays occur on the East coast.
- From Section 5.2, Section 5.3, and Section 5.4, we can see a general trend. I call it cascading delays. 
Shortest mean delays started in the morning or late morning and then delays get progressively longer at Late Night 
or Early Morning. This trend makes intuitive sense because if we had delays in the morning, then delays will be 
carried over in the next flight and cascaded as hours go by.
- I decided to check / drill down this hypothesis -- that delays are cascaded. I made 3 queries: query_1, 
query_2, and query_3. The query results surprised me and I have to reject the hypothesis. 300 minutes delays 
happened in the first or first two rows and happened in the Early Morning. Then flights generally returned to 
normalcy, i.e no delays as hours progressed.
- Then I explored causes of delays. I plot the causes of delays and it strengthens the rejection of the 
hypothesis -- that delays are cascaded. From the plot, we can see that delays are caused by LateAircraftDelay, 
CarrierDelay and WeahterDelay that happened longer at LateNight and EarlyMorning.