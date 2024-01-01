# Analyze A/B Test Results For E-Commerce Website

For this project, I worked on understanding the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. My goal is to work through the test results to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Table of contents

1. [Introduction to A/B testing](notion://www.notion.so/4d3468a7a97247858249890411e4384e#intro)
2. [Installation](notion://www.notion.so/4d3468a7a97247858249890411e4384e#installation)
3. [File Descriptions](notion://www.notion.so/4d3468a7a97247858249890411e4384e#files)
4. [Analysis](notion://www.notion.so/4d3468a7a97247858249890411e4384e#analysis)
5. [Results](notion://www.notion.so/4d3468a7a97247858249890411e4384e#observations)
6. [License](notion://www.notion.so/4d3468a7a97247858249890411e4384e#license)

## Introduction to A/B testing

![alt text](https://i.imgur.com/5PNPn3L.png)

A/B testing is one of the common technique used for analyzing which web designs drive more traffic. Many companies use A/B testing to test feature changes, layouts and even colors to increase a metric that measures a interest from the users.

The way this method works is, a group of people called `control group` is shown the old version of the web page and a group of people called `experiment group` is shown the new version of the web page. Based on how both groups respond, we can determine if new page is better and should be launched. It turns out that it is just an application of `Hypothesis Testing`.

We can set up hypothesis in this way (This is often related to what your problem is about):

- **`NULL`**: The new page is no better or worse than the old page.
- **`ALTERNATIVE`**: The new page is better than the old page.

Once we have our hypothesis set, we can use the data to see which hypothesis is supported.

## Installation

The following libraries and tools are used in this project:

- **`Numpy`**
- **`Pandas`**
- **`Statsmodels`**
- **`Matplotlib`**
- The code should run with no issues using Python version `3.*.`

## File Descriptions

This project contains the following files:

- **`ab_data.csv`**: holds the A/B test results data.
- **`countries.csv`**: Another file holding country information for each user in `ab_data.csv` file
- **`ABTestResultsForEcommerce.ipynb`**: Jupyter notebook containing Python code and briefly describing each step.
- **`ABTestResultsForEcommerce.html`**: HTML version of the notebook.

## Analysis

My analysis includes interpreting the A/B test results to suggest whether or not the E-Commerce company has to implement the new web page to increase conversion rate in the following ways:

- Using descriptive statistics
- Hypothesis Testing
- Z_test
- Logistic Regression

Please refer to the notebook for detailed info on how these individual analyses are performed.

## Results

These are the conclusions I found based on my analysis:

- According to the results from each analysis, all of them suggested sticking with the old web page as the increase in conversion rate with the new web page doesn't seem statistically significant.
- However, the results can alter if the A/B test is conducted longer.

## License

Licensed under [MIT License](https://github.com/ManideepTelukuntla/InvestigateTMDBMovieData/blob/master/LICENSE)
