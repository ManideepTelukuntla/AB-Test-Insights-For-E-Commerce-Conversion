# A/B Test Insights for E-Commerce Conversion

<div align="center">
  <img src="https://i.imgur.com/5PNPn3L.png" width="800" height="350" alt="Stock Portfolio Optimization">
  <br>
  <p>Image from imgur</p>
</div>

## Table of Contents
1. [Introduction/Overview](#1-introductionoverview)
2. [Objective](#2-objective)
3. [Methodology/Approach](#3-methodologyapproach)
4. [Installation/Requirements](#4-installationrequirements)
5. [File Descriptions](#5-file-descriptions)
6. [Data Collection and Sources](#6-data-collection-and-sources)
7. [Results/Conclusions](#7-resultsconclusions)
8. [License](#8-license)

## 1. Introduction/Overview
For this project, I worked on understanding the results of an A/B test run by an e-commerce website. The company has developed a new web page to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. My goal is to work through the test results to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## 2. Objective
To analyze A/B test results to determine the more effective web page design for increasing user conversion rates.

## 3. Methodology/Approach

A/B testing is one of the common technique used for analyzing which web designs drive more traffic. Many companies use A/B testing to test feature changes, layouts and even colors to increase a metric that measures a interest from the users.

The way this method works is, a group of people called `control group` is shown the old version of the web page and a group of people called `experiment group` is shown the new version of the web page. Based on how both groups respond, we can determine if new page is better and should be launched. It turns out that it is just an application of `Hypothesis Testing`.

We can set up hypothesis in this way (This is often related to what your problem is about):

- **`NULL`**: The new page is no better or worse than the old page.
- **`ALTERNATIVE`**: The new page is better than the old page.

Once we have our hypothesis set, we can use the data to see which hypothesis is supported.

My approach includes interpreting the A/B test results to suggest whether or not the E-Commerce company has to implement the new web page to increase conversion rate in the following ways:

- Using descriptive statistics
- Hypothesis Testing
- Z_test
- Logistic Regression

Please refer to the `ABTestResultsForEcommerce.ipynb` notebook for detailed info on how these individual analyses are performed.

## 4. Installation/Requirements
The following libraries and tools are used in this project:
- **Numpy**
- **Pandas**
- **Statsmodels**
- **Matplotlib**
- The code should run with no issues using Python version `3.*.`

## 5. File Descriptions
This project contains the following files:
- **`ab_data.csv`**: holds the A/B test results data.
- **`countries.csv`**: Another file holding country information for each user in `ab_data.csv` file
- **`AB-Test-Insights-For-E-Commerce-Conversion.ipynb`**: Jupyter notebook containing Python code and briefly describing each step.
- **`AB-Test-Insights-For-E-Commerce-Conversion.html`**: HTML version of the notebook.

## 6. Data Collection and Sources
This project contains two datasets:
- **`ab_data.csv`**: This file contains the A/B test results. The structure of the file is as follows
  #### File Structure
  - `user_id`: Unique identifier for each user
  - `timestamp`: The date and time when the user visited the page
  - `group`: Indicates whether the user was in the control or treatment group
  - `landing_page`: Shows the version of the page the user landed on (old_page or new_page)
  - `converted`: Indicates whether the user converted (1) or not (0)

- **`countries.csv`**: This file contains country information corresponding to each user in `ab_data.csv`. It helps in understanding geographical influences in the A/B test results.

## 7. Results/Conclusions
According to the analysis:
- All analyses suggested sticking with the old web page as the increase in conversion rate with the new web page doesn't seem statistically significant.
- The results can alter if the A/B test is conducted longer.

## 8. License
Licensed under [MIT License](https://github.com/ManideepTelukuntla/InvestigateTMDBMovieData/blob/master/LICENSE)
