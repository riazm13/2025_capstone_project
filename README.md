# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# Project XYZ

Project Title: Capstone_Project

Author: Mohammed Luqman Riaz

Dataset: transactions.csv 

## Dataset Content

The dataset used in this project is transactions_clean.csv, which contains structured records of customer transactions. Each row represents a single transaction and includes key attributes related to customer identification, purchase details, and transaction metadata.

File size & shape
File format: CSV (Comma-Separated Values)

Rows: X (to be filled from actual data)

Columns: Y (to be filled from actual data)

Size: Small enough to be processed locally and stored in a GitHub repository (well below the 100 GB limit).

Key Columns
Customer_ID — Unique identifier for each customer.

Transaction_ID — Unique identifier for each transaction.

Date — Date of the transaction.

Product / Service details — Information about what was purchased.

Amount — Monetary value of the transaction.

Payment Method — The mode of payment used.

Purpose of the Dataset
This dataset enables analysis of customer purchase patterns, transaction volumes, revenue trends, and behavior segmentation. It is also suitable for applying machine learning techniques, such as classification and regression, to predict outcomes like transaction amounts or customer segmentation.

Suitability
The dataset is cleaned (duplicates removed, missing values handled) and ready for advanced analytics. Its size makes it appropriate for:

Exploratory Data Analysis (EDA)

Visualisation with Python or BI tools like Tableau

Predictive modeling using Scikit-learn (decision trees, regression, classification)

Deployment in lightweight data apps (e.g., Streamlit)

## Business Requirements
* Describe your business requirements

Business Case / Problem Statement:
The purpose of this project is to analyze customer transaction data to identify trends, improve decision-making, and generate actionable insights for business growth.

Business Goals
Understand customer purchasing patterns

Identify the most popular products and services.

Track how frequently customers purchase and how much they spend.

Monitor revenue and transaction trends over time

Analyze sales performance by day, month, and season.

Detect revenue spikes and potential slow periods.

Segment customers for targeted marketing

Group customers based on purchase frequency, spending habits, and preferred payment methods.

Identify high-value customers for loyalty programs.

Improve operational efficiency

Detect anomalies in transactions, such as unusually high/low amounts.

Evaluate payment method usage to optimize payment processing.

Support strategic decision-making with predictive analytics

Predict potential high-value customers.

Forecast sales based on historical transaction data.

Key Questions to Answer
What are the top-selling products or services?

Which customers generate the most revenue?

Are there seasonal patterns in sales?

How do payment methods vary among customers?

Can we predict customer lifetime value based on historical transactions?

Deliverables
Interactive Dashboard (Streamlit):

Visualizing top products, revenue trends, customer segments, and payment method distribution.

Statistical Analysis:

Summary statistics, correlations, and hypothesis testing.

Predictive Models:

Simple machine learning models for sales forecasting and customer segmentation.









## Hypothesis and how to validate?
1. 
Certain payment methods are more common among high-value customers.

Validation Approach:

Compare payment method distribution between high-value and low-value customer segments.

Use a Chi-square test to determine if the difference in payment method usage is statistically significant.

2. 
High-value customers follow consistent purchasing patterns and can be predicted based on transaction history.

Validation Approach:

Perform RFM analysis (Recency, Frequency, Monetary Value) to classify customers into segments.

Use clustering (e.g., K-Means) to identify patterns among high-value customers.

Validate by comparing predicted high-value customers with actual top spenders in recent months.

3. 
Revenue shows seasonal trends, with certain months or periods generating higher sales.

Validation Approach:

Aggregate revenue by month and visualize trends using time-series plots.

Apply seasonal decomposition to detect recurring patterns.

Conduct a statistical test (e.g., Kruskal-Wallis) to confirm significant differences between months.



## Project Plan
1. Data Collection
The dataset transactions_clean.csv was sourced from internal transaction logs (or an equivalent public dataset).

Data was obtained in CSV format and stored in the project’s /Data_set/ directory for reproducibility.

Original dataset underwent an initial review to understand its structure, key variables, and potential analytical value.

2. Data Management & Processing
Loading & Inspection: Loaded into Python using pandas for inspection of data types, missing values, and duplicates.

Cleaning:

Removed duplicate transaction_id and customer_id entries.

Handled missing values via imputation or removal based on the field’s importance.

Converted date columns to datetime objects.

Normalized categorical fields (e.g., payment method names).

Storage:

Saved a cleaned version as transactions_clean.csv for consistent use across analysis, visualization, and modeling stages.

Version control managed through GitHub.

3. Exploratory Data Analysis (EDA)
Visualizations created with matplotlib and seaborn to understand:

Transaction volume trends over time

Distribution of transaction amounts

Most popular products/services

Customer segmentation patterns

Payment method preferences

Statistical Analysis performed to identify correlations, outliers, and seasonal patterns.

4. Machine Learning (Tree-Based Models)
Goal: Predict transaction class (e.g., high/low value) and explore revenue prediction.

Models Used: Decision Tree Classifier and Random Forest Regressor from scikit-learn.

Feature Engineering:

Extracted features from transaction date (day, month, weekday, hour).

Created aggregated customer-level metrics (recency, frequency, monetary value).

Model Evaluation:

Train-test split for unbiased evaluation.

Accuracy, Precision, Recall for classification.

RMSE and R² for regression.

Model Visualization:

Decision tree plots

Feature importance charts

5. Interpretation & Insights
Models and visualizations used to answer business questions such as:

Which customers are most valuable?

Which products generate the most revenue?

Can we forecast revenue or classify future high-value transactions?

Actionable recommendations documented based on findings.

6. Research Methodology Choice
Exploratory Analysis chosen first to build an intuitive understanding of the dataset.

Tree-Based Models selected for their interpretability, ability to handle mixed data types, and feature importance insights.

Statistical Testing integrated to validate observed trends with evidence.

Iterative Development applied: cleaning, analysis, modeling, and refinement repeated as new insights emerged.

## The rationale to map the business requirements to the Data Visualisations
The rationale to map the business requirements to the Data Visualisations
The project aims to deliver actionable insights to stakeholders by aligning each business requirement with the most suitable data visualisation method. This mapping ensures that every stakeholder question can be answered through clear, intuitive, and data-driven visuals.

1. Identify top-selling products and categories

Rationale: Stakeholders require a clear understanding of which products or categories drive the most revenue to optimise inventory and marketing campaigns.

Visualisation Choice: Bar Chart and Pareto Chart — Bar charts clearly show top performers, while Pareto charts highlight the 80/20 distribution for prioritisation.

2. Understand sales trends over time

Rationale: Monitoring seasonal and monthly fluctuations in sales can guide promotional strategies and resource allocation.

Visualisation Choice: Line Chart — Best suited for showing temporal patterns and seasonal peaks/troughs in transaction volume or revenue.

3. Analyse customer purchasing behaviour

Rationale: Understanding buying frequency and spending habits helps tailor loyalty programs and personalised recommendations.

Visualisation Choice: Histogram and Boxplot — Histograms reveal purchase frequency distribution, while boxplots identify outliers and median spending patterns.

4. Detect geographic sales performance

Rationale: Regional insights inform targeted marketing, logistics, and supply chain decisions.

Visualisation Choice: Geographic Heatmap — Highlights sales intensity across locations for easy spatial pattern recognition.

5. Predict future sales using machine learning

Rationale: Forecasting sales helps with inventory planning, budgeting, and capacity management.

Visualisation Choice: Regression Plot (Predicted vs. Actual) and Feature Importance Chart — Show model accuracy and which variables most influence predictions.

6. Classify high-value customers

Rationale: Identifying and targeting customers with high lifetime value improves retention and revenue growth.

Visualisation Choice: Decision Tree Plot and Confusion Matrix — Decision trees visualise classification logic, while confusion matrices show model performance.

By mapping requirements to the right visualisation types, the dashboard ensures that both technical and non-technical stakeholders can quickly interpret insights and act upon them.

## Analysis techniques used
Data Analysis Methods Applied

Data Cleaning & Preprocessing

Removed duplicate transaction IDs and customer IDs.

Handled missing values using deletion for incomplete records and imputation where appropriate.

Normalised inconsistent date formats and ensured numeric columns were properly typed.

Exploratory Data Analysis (EDA)

Descriptive statistics to understand central tendencies and dispersion.

Visual exploration with histograms, bar plots, heatmaps, and time-series plots to uncover trends and anomalies.

Segmentation & Classification

RFM Analysis to segment customers based on recency, frequency, and monetary value.

Decision Tree Classifier to identify rules for high-value customer classification.

Regression Modelling

Used Decision Tree Regressor to predict sales/revenue based on transaction features.

Feature importance ranking to identify key drivers of sales.

Time-Series Analysis

Aggregated sales by month to detect seasonal patterns.

Checked for trends using moving averages.

Limitations and Alternative Approaches

Limitation: Dataset size and structure limited the complexity of models; some variables (e.g., marketing campaigns, promotions) were absent.

Alternative Approach: Could integrate external data (e.g., holidays, weather, competitor pricing) to improve predictive power.

Limitation: Tree-based models can overfit small datasets.

Alternative Approach: Use Random Forest or Gradient Boosting for better generalisation.

Structuring the Analysis Techniques

The workflow followed a pipeline structure:
Data Cleaning → EDA → Feature Engineering → Model Training → Evaluation → Insights.

This ensured reproducibility and allowed iterative improvement of models and visualisations.

Use of Generative AI Tools

Ideation: Used AI to brainstorm hypotheses, business requirements, and mapping to visualisations.

Design Thinking: Collaborated with AI to design dashboards and choose visualisation types based on user stories.

Code Optimisation: AI-generated base code for data cleaning, visualisation, and ML models, which was then reviewed and refined for efficiency and readability.

## Ethical considerations
Data Privacy

Customer IDs were anonymised numeric codes; no personally identifiable information (PII) was exposed.

No attempt was made to deanonymise or link customers to external datasets.

Bias and Fairness

Potential bias exists if historical sales reflect unequal market reach or limited geographic coverage.

Models were tested to ensure performance did not disproportionately favour one region or customer segment.

Legal and Societal Issues

The dataset aligns with GDPR principles since it contains no direct identifiers.

Care was taken not to present data in a way that could harm specific customer groups or imply discriminatory practices.

Mitigation Actions

Used aggregated data in visualisations to prevent singling out individuals.

Validated model fairness by checking classification performance across different geographic and demographic segments where possible.
## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Deployment
The deployment process is carried out using Tableau.
Link: https://public.tableau.com/views/CapstoneProject_17549184048650/Story1?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link   


## Main Data Analysis Libraries
In this project, I utilized several essential Python libraries for data analysis, visualization, and machine learning. Pandas was primarily used for data loading, cleaning, and manipulation, allowing me to efficiently handle tabular data from CSV files. NumPy complemented this by providing support for numerical operations and array handling. For data visualization, Matplotlib and Seaborn were employed to create informative plots, such as histograms and boxplots, which helped in understanding the data distribution and relationships between variables. For predictive modeling, I leveraged the scikit-learn library, using tools like train_test_split for dividing the data into training and testing sets, and LabelEncoder for converting categorical variables into numeric format suitable for modeling. I implemented decision tree and random forest algorithms, both classifiers and regressors, to build predictive models. Finally, model performance was evaluated using metrics such as confusion matrices for classification and mean squared error and R² score for regression tasks, with visualizations aiding in interpreting the results.



## Credits 

Content and Code Assistance
I utilized several AI-powered tools to assist with code generation, explanation, and overall project development. Specifically, I relied on ChatGPT, Grock AI, and the built-in Copilot feature to help write, debug, and optimize the code throughout this project. These tools were instrumental in breaking down complex elements, allowing me to understand and implement solutions more quickly and accurately. Additionally, I used resources available through the Learning Management System (LMS) for guidance and supplementary material. This combined support enabled me to efficiently complete the project while maintaining high-quality results.

CI: I also found help in asking the CI's for help alot as they helped me to get back on track when I was having alot of issues.


## Acknowledgements (optional)
I would like to express my deepest gratitude to Emma for her exceptional guidance and support in helping me navigate the complexities of machine learning. Her expertise and encouragement were instrumental in my learning journey. I also extend my sincere thanks to all the course instructors, whose dedication and knowledge made this experience truly enriching. Additionally, I am profoundly grateful to my parents for their unwavering patience and support throughout this challenging assignment, which made it possible for me to persevere and succeed.