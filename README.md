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
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations
* Were there any data privacy, bias or fairness issues with the data?
* How did you overcome any legal or societal issues?

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
### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.


## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.