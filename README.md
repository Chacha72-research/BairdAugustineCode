Hey everyone! My name is Charan, an incoming Information Management and Statistics sophomore at UC Santa Cruz. With the help of Python, Yahoo Finance, and Google Sheets, I’m developing a project that compiles valuation information on the public SaaS (Software as a Service) landscape to help investors value private SaaS firms. (172+ Public SaaS companies!!) Public trends in publicly traded SaaS companies are usually a big indicator of how much value a new and upcoming private SaaS firm can create. 

I want to leverage data science, machine learning, and corporate valuation principles such as the discounted cash flow model, to create a valuable tool to investors in this project.

This project involves data collection, analysis of the whole SaaS industry based on this datga, and using the information I collected to create a "partial" Discounted Cash Flow Analysis machine learning model, helping investors take out assumptions in forecasting cash flows when valuing businesses. The DCF model is one of the most important valuation principles, and I hope to leverage that in this project. More information inside my code notebooks!

Here’s an overview of everything I’ve done! (So far!)

I first started by utilizing the =GOOGLEFINANCE command on Google Sheets to compile basic company information (i.e Market Cap, Profit Margin) based on their tickers, as well as using a public SaaS company database I found. Here is the comprehensive spreadsheet of these values:
https://docs.google.com/spreadsheets/d/1eJjBRiNbxmXz46NK0kBK_lSnL67r07sgCjXFRDalDFI/edit?usp=sharing 

The rest of my project and explanations can be found in each code notebook. Take a look at the rest of my project in this order.

Data Collection Folder:
1. Valuation Metrics
2. Exploratory Analysis
3. Partial-DCF ML Model Processing

Models Folder:
1. Neural Network + Random Forest Model Training (Deep Learning Models)
2. Polynomial Regression Modeling for future Values
3. Putting it all together: Using saved deep learning models for predicting unlevered free cash flows for next 3 years

I compiled a bunch of key insights from my data:
https://docs.google.com/document/d/1DjHiHK9KNZ35h3IX4NQttNDcuIKvfV4gLdmymOlWx-s/edit?usp=sharing 

--> Which I then used to create a comprehensive Tableau Story Dashboard on top SaaS companies and their key insights here: 
https://public.tableau.com/views/BairdAugustineFinalDataProject/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link 

This dashboard is always being updated with new information and more companies from the public SaaS firm list!


Future updates with project:
- Refine organization with a repository of key spreadsheets and CSV files used throughout the code.
- Improve model accuracy, and improve Tableau Dashboard with more detail.

Thanks for taking the time to look through my project! Please feel free to email me at: crameshk@ucsc.edu for further questions.


**Credits to EODHD Financial API and yfinance API for project data**


Additional Data Used:
https://docs.google.com/spreadsheets/d/1MeeeVvYWWZYqgge2MPyxj_VMEBmVgPVltq3V4NXZH_E/edit?gid=1211987008#gid=1211987008 
