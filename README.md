# Analyze A/B Test Results For E-Commerce Website

For this project, I will be working to understand the results of an A/B test run by an e-commerce website. The company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product. My goal is to work through the test results to help the company understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Table of contents
1. [Introduction to A/B testing](#intro)
2. [Installation](#installation)
3. [File Descriptions](#files)
4. [Analysis](#analysis)
5. [Results](#observations)
6. [License](#license)

## Introduction to A/B testing
![A/B Testing](https://i.imgur.com/5PNPn3L.png)
A/B testing is one of the common technique used for analyzing which web designs drive more traffic. Many companies use A/B testing to test feature changes, layouts and even colors to increase a metric that measures a interest from the users.

The way this method works is, a group of people called `control group` is shown the old version of the web page and a group of people called `experiment group` is shown the new version of the web page. Based on how both groups respond, we can determine if new page is better and should be launched. It turns out that it is just an application of `Hypothesis Testing`.

We can setup hypothesis in this way (This is often related to what your problem is about):
- **`NULL`**: The new page is no better or worse than the old page.
- **`ALTERNATIVE`**: The new page is better than the old page.

Once we have our hypothesis setup we can then use the data to see which hypothesis is supported.

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
- **`ABTestResultsForEcommerce.ipynb`**: Jupyter notebook containing python code and brief description about each step.
- **`ABTestResultsForEcommerce.html`**: HTML version of notebook.

## Analysis
My analysis includes interpreting the A/B test results inorder to suggest whether or not E-Commerce company has to implement the new web page to increase conversion rate in the following ways:
- Using descriptive statistics
- Hypothesis Testing
- Z_test
- Logistic Regression

Please refer to the notebook for detailed info on how these individual analysis are performed.

## Results
These are the conclusions I found based on my analysis:
- According to the results produced from each analysis I have performed, all of them suggested to stick with the old web page as the increase in conversion rate with new web page does'nt seem to be statiscally significant.
- However the results can alter if the A/B test is conducted for longer duration.

## License
Licensed under [MIT License](https://github.com/ManideepTelukuntla/InvestigateTMDBMovieData/blob/master/LICENSE)
