# Data analysis process

# Steps of the analysis process

## Asking a question

Typically its a question reflecting a problem/issue an organisation needs resolved

A good data question is specific, includes guidance on the who, what how much, etc of the analysis

## Getting the data

This starts by selecting and evaluating data, when doing so, there are some questions that need answering to determine if it will bee useful in answering the original data question. The questions are:

- Who collected the data?
- What data is included?
- When was it collected?

- Where has it come from?
- Why was it collected?

### Who collected the data?

- Considering how credible the collector is
- Evaluation of biases in collection methods
- Assessment of if the collector follows industry standards

*For example, data from an established analytics platform vs. informal surveys*

### What data is included?

Examining the content & completeness of the dataset

- Checking for relevant KPI’s & Metrics
- Verifying data completeness & accuracy
- Ensuring data aligns with project objectives

*For example, user interaction data should include timestamps, actions and context*

### When was it collected?

Timing is integral for analysing data

- Check data collection dates & frequency
- Assessing if the data reflects current trends
- Considering technological changes since collection

*For example, an old dataset may not be any good to analyse recent trends*

### Where did it come from?

- Verifying source credibility
- Checking data collection methods
- Confirming data security & compliance

*for example, user engagement data likely would be more reliable than survey reported data*

### Why was it collected?

- Understanding the original collection purpose
- Assessing relevance to the objectives
- Considering ethical implications of re-purposing the data

## Preparing the data

Preparing the data for analysis & exploration

- Extracting data from its source - May involve writing SQL queries to extract & transform the data from a database or downloading from an external source
- Transforming/organising the data - Involves summarising the data, joining data from different sources, `and putting it into a format that's accessible in the tool being used to explore it
- Cleaning the data - Involves removing duplicate data, correcting inaccurate or missing data, reformatting columns & dealing with outliers

## Exploring the data

Commonly called ‘exploratory data analysis’ or EDA

Exploring the data isn’t arriving at a final answer to the data question, this is done to understand the data & uncover patterns/interesting features in a dataset

This also helps to determine what should be addressed later in the data analysis process

Often descriptive statistics are used by analysts to understand the data, this is a way to summarise or aggregate large datasets into lists or numbers. Helping to describe datasets in a more meaningful/interpretative way

- We could start by calculating the minimum, median, average, and maximum of all quantitative variables.
- For qualitative variables, we can use frequency tables to understand their distribution.
- A frequency table counts the number of times each unique value appears in a column.

### Mean, Mode & Median averages

Mean - Fount by adding all numbers and dividing by how many numbers there are

Median - Middle value when all numbers are arranged in order

Mode - Value that appears most often in a dataset

## Exploring the data

- Data visualisation - Displays quantitative & qualitative data for quick interpretation, visuals can help you quickly see the distributions or trends in data

*For example, rather that relying on average, max and min, a histogram could be used*

- Histograms are column charts where each column shows the number of values that appear within the range of values for that column.
- For example, the value for the second bar is 358, meaning there are 358 employees with a monthly income between 2,009 and 3,009.
- With this chart, you can see a more complete picture of the distribution of monthly salaries.
- Histograms work great for quantitative variables but not qualitative variables.
- To see the distribution of qualitative variables, we can use a simple bar chart.

## Analysing the data

- The fourth stage in the data analysis process is to **Analyse the data**.
- In this stage, data professionals extract insights from data to guide their decision-making.
- The data field commonly identifies four levels of data analysis, which work together to help organisations and individuals make data-driven decisions.
- In increasing order of complexity or sophistication, the four levels of data analysis are: descriptive, diagnostic, predictive, and prescriptive.

### Descriptive analysis

- Descriptive analysis uses past data to answer the question What happened?
- Previously collected data undergoes analysis to answer key questions about past situations or events.
- For example, a company would use descriptive analysis to determine which products generated the highest volume of sales in the previous year, or which employees demonstrated the greatest productivity.

### Diagnostic analysis

- Diagnostic analysis seeks reasons or explanations for what has happened, asking and answering the question Why did this occur?
- It is often difficult or impossible to prove cause and effect, diagnostic analysis tends to explore correlations and other relationships in data.
- For example, medical researchers have long sought to determine what causes multiple sclerosis.
- They have found a strong association between the incidence of the Epstein-Barr virus and multiple sclerosis, leading them to hypothesise that exposure to the Epstein-Barr virus may explain subsequent multiple sclerosis diagnoses.

### Predictive analysis

- Predictive analysis uses past data to predict future occurrences or unknown values. It addresses the question What is likely to happen in the future?
- It uses statistical methods and machine learning to identify trends, patterns, and relationships in the data.
- Predictive analysis is commonly used to forecast customer behaviour, credit card default and fraud, market trends, labour demand, weather events, and other important business and social outcomes of interest.

### Prescriptive analysis

- Prescriptive analysis is the most sophisticated of the four levels, using historical data to address the question What should we do?
- It analyses data and generates advice on possible outcomes for different decisions, helping guide decision-makers toward action.
- Prescriptive analysis helps to automate future decisions, such as evaluating the creditworthiness of a borrower.

## Modelling