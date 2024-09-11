## SaaS Valuation Tool Project - README

My name is Charan Rameshkumar, an incoming sophomore at UC Santa Cruz, and here is my SaaS Valuation Project associated with BairdAugustine's internship program.

**Project Overview:**
This project aims to provide investors with insights into the public SaaS (Software as a Service) landscape, helping them to better evaluate and forecast the value of new and upcoming private SaaS firms. By analyzing trends in public SaaS companies, this tool leverages corporate valuation principles—most notably the **Discounted Cash Flow (DCF) model**—to make more accurate predictions about the future cash flows of SaaS companies.

### Key Goals:
1. **Public SaaS Company Insights**: Provide investors with a detailed overview of how large public SaaS companies are performing across several key metrics. The data is visualized through a **Tableau dashboard**, which offers an intuitive way to track these trends and support investment decisions in new and emerging private SaaS firms.
2. **Forecasting Future Cash Flows**: Equip investors with a machine learning tool that forecasts **unlevered free cash flows (UFCF)** for private SaaS firms. These forecasts are based on models trained using data from over 170 public SaaS companies, removing some of the guesswork from traditional financial models.

### Project Features:
- **Data Collection**: Using Python, I built web scrapers to pull data from APIs like Yahoo Finance (`yfinance`) and EODHD Financial API. The data collected includes financial statements, cash flow trends, and various valuation metrics.
- **Exploratory Data Analysis (EDA)**: I utilized **NumPy**, **pandas**, and **matplotlib** to analyze and clean the data, producing over 15 visualizations. This analysis provides insights into the financial health and performance of these companies.
- **Machine Learning Models**: I developed and trained **deep learning models** (using **TensorFlow**, **Keras**, and **scikit-learn**) to predict **unlevered free cash flows (UFCF)**. These models are designed to assist investors in applying the DCF framework more effectively.

### How to Read and Understand this Project in Order: (each notebook also has markdown text to help explain my processes and coding procedures)
1. Look Through **Data Collection** in this order:
     - **Valuation Metrics**: Raw financial and company data sourced from APIs.
     - **Exploratory Analysis**: Visualizations and initial insights.
     - **Partial-DCF ML Model Processing**: Preprocessing steps for training the DCF forecasting models.
   
2. Look Through **Modeling** in this order:
     - **Neural Network + Random Forest Model Training**: Deep learning models and random forest for robust cash flow prediction.
     - **Polynomial Regression Modeling**: Alternative regression models for comparison and future value prediction.
     - **Putting it All Together**: Integration of saved models for UFCF prediction over the next three years.

3. **Visualization**:
   - Access the **Tableau Dashboard** here: [https://public.tableau.com/views/BairdAugustineFinalDataProject/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link](https://public.tableau.com/views/BairdAugustineFinalDataProject/Story1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link). This is a constantly updated visualization of key metrics for public SaaS companies, designed to help investors make informed decisions about upcoming SaaS firms.

### Key Insights:
Some key insights can be found in the [compiled document](https://docs.google.com/document/d/1DjHiHK9KNZ35h3IX4NQttNDcuIKvfV4gLdmymOlWx-s/edit?usp=sharing), which are also integrated into the **Tableau Story Dashboard**.

### Tools & Technologies:
- **Languages**: Python (NumPy, pandas, matplotlib, TensorFlow, Keras, scikit-learn)
- **APIs**: `yfinance`, EODHD Financial API
- **Visualization**: Tableau
- **Machine Learning**: Deep Learning, Random Forests, Polynomial Regression

### Future Work:
- **Repository Organization**: Organizing and refining the spreadsheets and CSV files used throughout the project.
- **Model Accuracy**: Continuously improving model accuracy and adding more detailed metrics to the Tableau dashboard.

### Data Sources:
- **Primary Data Collection**: Yahoo Finance via `yfinance` and EODHD Financial API.
- **Supplementary Data**: Additional data from [https://docs.google.com/spreadsheets/d/1MeeeVvYWWZYqgge2MPyxj_VMEBmVgPVltq3V4NXZH_E/edit?gid=1211987008#gid=1211987008](https://docs.google.com/spreadsheets/d/1MeeeVvYWWZYqgge2MPyxj_VMEBmVgPVltq3V4NXZH_E/edit?gid=1211987008#gid=1211987008).

Feel free to reach out to me at **crameshk@ucsc.edu** with any questions or suggestions!

---

**Credits**:
- Data provided by Yahoo Finance, EODHD Financial API, and public SaaS firm databases.
- Special thanks to **Google Sheets** for providing a quick way to start data collection via `=GOOGLEFINANCE`.
- Special thanks to everyone at BairdAugustine for providing suggestions on better metrics and visualization tips :)

