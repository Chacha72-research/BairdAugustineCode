Hey everyone! My name is Charan, an incoming Information Management and Statistics sophomore at UC Santa Cruz, super interested in data and finance. With the help of Python, Yahoo Finance, and Google Sheets, I’m developing a project that compiles valuation information on the public SaaS landscape to help investors value private SaaS firms. I want to make this information and tools associated with the project as digestible and valuable as possible, so every investor can use this project to make good decisions. The code outline was formed using AI tools and YouTube tutorials for direction (with high error LOL!) , but heavily repurposed and redeveloped to fit the needs of this project and to fit the needs of investors.

Here’s an overview of everything I’ve done! (So far!)

I first started by utilizing the =GOOGLEFINANCE command on Google Sheets to compile basic company information (i.e Market Cap, Profit Margin) based on their tickers, as well as using a public SaaS company database I found. Here is the comprehensive spreadsheet of these values:
https://docs.google.com/spreadsheets/d/1eJjBRiNbxmXz46NK0kBK_lSnL67r07sgCjXFRDalDFI/edit?usp=sharing 

Then, I started compiling information on particular valuation metrics per company. However, =GOOGLEFINANCE didn’t have the capability to get these particular values, so I created various Python scripts that scraped YahooFinance to calculate these values. It also helped with automating the process of finding information on companies, since there are over 170 of them. All these metrics can be found here: https://docs.google.com/spreadsheets/d/1SEIanQtt9br6DuvXBDwuDBxG6fgJOGQDPQ9UH_P7HAU/edit?usp=sharing 

After compiling this information, I came across the concept of the Discounted Cash Flow model, helpful in predicting a company’s future cash flows in terms of today’s money based on various assumptions and a discount rate. However, I wanted to develop a tool that could take out the assumptions in the cash flow model. Since future cash flows are assumed, I wanted to develop a machine learning model (a neural network) that could take Yahoo Finance financial statements, as well as the previously compiled information to predict cash flows for the next 5 years. 

Here’s how machine learning models work on a high level. The general gist is that models work by learning from training data and evaluating itself on testing data.

In machine learning, training data is used to teach a model how to make predictions. This data includes both input features and the correct outputs, allowing the model to learn patterns and relationships. In a simple example, you could give a model pictures of various colors and tell it, “this is red,” or “this is not red.” Once trained, the model can tell which picture is red.

In our DCF instance, if you’re training a model to predict future cash flows, you’d provide it with historical data on revenue, EBITDA, and other financial metrics along with actual cash flow outcomes. The model learns from this data to understand how these factors influence cash flow.

After training, the model is evaluated using testing data, which consists of new, unseen examples. This step is crucial to check how well the model generalizes its learning to different data. For example, after training your cash flow model on historical financial data, you’d test it with data from other companies not included in the training set to see if it can accurately predict cash flows. This evaluation helps ensure that the model performs well beyond the specific examples it was trained on.

And so, this is the approach I used! It worked surprisingly well with a ~92% accuracy, with predictions being off by 1 million dollars in the context of 10 billion dollar values, and a loss of 20000 dollars in the context of million dollar values. (which is pretty awesome!!)

Here’s the historical data I used, along with finance API’s historical financial statement data: https://docs.google.com/spreadsheets/d/1MeeeVvYWWZYqgge2MPyxj_VMEBmVgPVltq3V4NXZH_E/edit?usp=sharing 

I compiled a bunch of key insights from my data:
https://docs.google.com/document/d/1DjHiHK9KNZ35h3IX4NQttNDcuIKvfV4gLdmymOlWx-s/edit?usp=sharing 

Finally, I wanted to visualize my data, so that anyone can look at the key insights as well as charts to make better decisions. I created a Tableau dashboard that took all my information and generated some pretty cool graphs. As a bonus, I even coded up a Google Search Trend script, which evaluates search trends of consumers with each of these SaaS companies. (Right now, it is a bit messy and doesn’t include a lot of the valuation metrics, but it should get updated by the end of this month)

Here are some of the factors that I’ve visualized so far. I hope to shorten the dashboard and make it more concise soon.
Market Cap x Company Bar Graph
Company x YoY Change in EBITDA Bar graph
Density Map of all Public SaaS companies
Box Plot Distribution of all Revenue Multiples
Pre-Pandemic vs. Current Stock Prices bar graph (to be added)
Largest Positive change in stock price from before the pandemic heat map
Largest Negative change in stock price from before the pandemic heat map
Pre-IPO investor heat map
Company Yearly growth in percent table
Revenue vs. Employee Count Scatter Plot
EBITDA Margin Histogram
Revenue Growth vs. EBITDA Growth Bubble Diagram
Stock Performance since 2023 line chart & Google search trend since 2023 line chart
Current Market Cap vs. Pre-IPO funding bar graph
Change in EBITDA vs. Yearly growth percent bar graph

https://public.tableau.com/shared/FB42Y8KJC?:display_count=n&:origin=viz_share_link 


Future Goals with Project:
Create Slide Deck with company information, investments and acquisitions, and valuation ratios to give a concise overview of public trends


