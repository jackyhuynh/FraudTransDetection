# Fraud-Transactions Detection System

## Introduction
The project focus on creating Fraud Detection Application to detect fraudulent credit card transactions. Thus, consumers and credit card companies are not paying for items that they did not purchase. According to Macaraeg (2019), the predicted worldwide non-cash transition growth from 2016 to 2020 is 12.7%. The increase in non-cash transactions leads to an increase in fraudulent transactions (Macaraeg, 2019). Even with EMV smart chips being implemented, the amount of money lost from credit card fraud is still very high. Therefore, implemented fraud detection (using data mining) is important. I also included 50 pages of fraud research (by myself) that can be found [ here](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/Report.pdf).

![alt](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/picture/testTable.PNG)

My application will be built from various data mining model and prediction methods. The combination of them will increase the change to prevent fraud detection. The disadvantage of this is the response time to end-users as many layers of detection will add more execution time to the application (O(log(n))).
Please click [here](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/Report.pdf) for the full statistic and prediction. 

![alt](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/picture/operationDiagram.PNG)

### Technology
* Business Analyst
* Machine Learning
* Data Mining
* Data Visualization
* HTML
* CSS
* AI

### Algorithm & Methods
* Data Exploration: Explore min, max, mean, standard deviation, correlation, and else.
* Data Transformation
* Plotting Methods
* Principal Component Analysis (PCA)
* Eigen Vector
* Hopskin Statistic
* Confusion Matrix
* Elbow method (for Utility Clustering)
* General Linear Algorithm (Predictive Model)
* Logistic Regression Algorithm (Predictive Model)
* Decision Tree Algorithm (Predictive Model)
* Random Forest Algorithm (Predictive Model)
* Support-Vector Machines Algorithm (Classification and Regression analysis)

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Data
Please download data at [kaggle.com](https://www.kaggle.com/mlg-ulb/creditcardfraud) first.

### Prerequisites
What things you need to install the software and how to install them:
- R CRAN Project: R is a free software environment for statistical computing and graphics. It compiles and runs on a wide variety of UNIX platforms, Windows and macOS
- RStudio IDE: RStudio is an integrated development environment (IDE) for R. It includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging, and workspace management. Click here to see more RStudio features. RStudio is available in open source and commercial editions and runs on the desktop (Windows, Mac, and Linux) or in a browser connected to RStudio Server or RStudio Server Pro (Debian/Ubuntu, Red Hat/CentOS, and SUSE Linux)

### Installing

A step by step series of examples that tell you how to get a development environment running:
* [Install R](https://www.r-project.org/) - If you haven't downloaded and installed R, here's how to get started.
* [R Studio IDE](https://rstudio.com/products/rstudio/#:~:text=RStudio%20Take%20control%20of%20your%20R%20code%20RStudio,tools%20for%20plotting,%20history,%20debugging%20and%20workspace%20management.) - After that choose R Studio Desktop, and the free version (unless you have the Pro install). R free version is a pretty good IDE.

## Running the tests

### Data
Please download data at [kaggle.com](https://www.kaggle.com/mlg-ulb/creditcardfraud) first.

Explain how to run the automated tests for this system:
- Start R Studio.
- Create new a project.
- Copy the data and markdown file (.rmd) into the source file. For example:
```
~/Fraud-TransactionsDetectionSystem/markdown.rmd
~/Fraud-TransactionsDetectionSystem/data.csv
```

- you can store the WholesaleCustomersData.csv in the same folder, but it is recommended to store in a data as below (coding standard):
```
~/Fraud-TransactionsDetectionSystem/data/data.csv
```

- Make sure to change the import code on top if you want to move your data anywhere. Depend on where you download the code. Your path will be different from mine. Please replace the path below with your  path:
```
# Import Data
Rdata <- read.csv("~/R/DataMining/FaultAnalyst.CreditCard/data/data.csv", header=TRUE)
# path:"~/R/DataMining/FaultAnalyst.CreditCard/data/data.csv"
```

- Please take a quick view of [import data in R](https://support.rstudio.com/hc/en-us/articles/218611977-Importing-Data-with-RStudio?mobile_site=true) if you fail to change the import code.
- Run the IDE by Choose the Knit option:
```
hit the "Knit" button
```
### Data Visualization:

Using cluster analysis, we can see some hypothesis. According to the density-chart, fraud transactions happened from 0 to 8 AM (early morning and during sleep time) while non-fraud transactions happen during active-time. This is also common sense since humans usually purchase in the daytime, not when they sleep. Therefore, transactions that happen at night (peak at 3 PM) have more chances to happen in fraud-transactions. There are 10 more plots and thousands of tests. Please click [here](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/Report.pdf) for the full report.

![alt](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/picture/transactionHours.PNG)


## Deployment
This can be deployed to any database system for inventory prediction. Please note the application will work with any bigger or smaller data set as long as it follows the design pattern of this data set.
```
## 'data.frame': 284807 obs. of 32 variables: 
## $ Time : num 0 0 1 1 2 2 4 7 7 9 ... 
## $ V1 : num -1.36 1.192 -1.358 -0.966 -1.158 ... 
## $ V2 : num -0.0728 0.2662 -1.3402 -0.1852 0.8777 ... 
## $ V3 : num 2.536 0.166 1.773 1.793 1.549 ... 
## $ V4 : num 1.378 0.448 0.38 -0.863 0.403 ... 
## $ V5 : num -0.3383 0.06 -0.5032 -0.0103 -0.4072 ... 
## $ V6 : num 0.4624 -0.0824 1.8005 1.2472 0.0959 ... 
## $ V7 : num 0.2396 -0.0788 0.7915 0.2376 0.5929 ... 
## $ V8 : num 0.0987 0.0851 0.2477 0.3774 -0.2705 ... 
## $ V9 : num 0.364 -0.255 -1.515 -1.387 0.818 ... 
## $ V10 : num 0.0908 -0.167 0.2076 -0.055 0.7531 ... 
## $ V11 : num -0.552 1.613 0.625 -0.226 -0.823 ... 
## $ V12 : num -0.6178 1.0652 0.0661 0.1782 0.5382 ... 
## $ V13 : num -0.991 0.489 0.717 0.508 1.346 ... 
## $ V14 : num -0.311 -0.144 -0.166 -0.288 -1.12 ... 
## $ V15 : num 1.468 0.636 2.346 -0.631 0.175 ... 
## $ V16 : num -0.47 0.464 -2.89 -1.06 -0.451 ... 
## $ V17 : num 0.208 -0.115 1.11 -0.684 -0.237 ... 
## $ V18 : num 0.0258 -0.1834 -0.1214 1.9658 -0.0382 ... 
## $ V19 : num 0.404 -0.146 -2.262 -1.233 0.803 ... 
## $ V20 : num 0.2514 -0.0691 0.525 -0.208 0.4085 ... 
## $ V21 : num -0.01831 -0.22578 0.248 -0.1083 -0.00943 ... 
## $ V22 : num 0.27784 -0.63867 0.77168 0.00527 0.79828 ... 
## $ V23 : num -0.11 0.101 0.909 -0.19 -0.137 ... 
## $ V24 : num 0.0669 -0.3398 -0.6893 -1.1756 0.1413 ... 
## $ V25 : num 0.129 0.167 -0.328 0.647 -0.206 ... 
## $ V26 : num -0.189 0.126 -0.139 -0.222 0.502 ... 
## $ V27 : num 0.13356 -0.00898 -0.05535 0.06272 0.21942 ... 
## $ V28 : num -0.0211 0.0147 -0.0598 0.0615 0.2152 ... 
## $ Amount : num 149.62 2.69 378.66 123.5 69.99 ... 
## $ Class : Factor w/ 2 levels "one","zero": 2 2 2 2 2 2 2 2 2 2 ... 
## $ hour_of_day: num 0 0 0.000278 0.000278 0.000556 ...
```
More continuous attributes can just be added to the application, and it should work fine (with a bit of modification). Please refer to my research paper for a better understanding. [Full research paper can be found here](https://github.com/jackyhuynh/salePredictionModels-dataMining/blob/main/src/Markdown-WholeSale.pdf).

I will not guarantee that this application will work "Big data set". If you are interested in a "Big(or Large) data set" please join here for [an argument](https://www.researchgate.net/post/How-much-data-is-considered-to-be-small-data-Large-data-in-data-mining) on what data set is considered a large data set in data mining.

## Built With

* [R Studio IDE](https://rstudio.com/products/rstudio/#:~:text=RStudio%20Take%20control%20of%20your%20R%20code%20RStudio,tools%20for%20plotting,%20history,%20debugging%20and%20workspace%20management.) 
* [R CRAN Project](https://www.r-project.org/)

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags). 

## Authors

* **Truc Huynh** - *Initial work* - [TrucDev](https://github.com/jackyhuynh)

## References

my README.md format was retrieved from
* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* Hat tip to anyone who's code was used
* Inspiration
* etc
* **Purdue University FortWayne** - where I represent this research in presentation and get improved feedback.

