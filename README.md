# Fraud-Transactions Detection System

## Introduction
The project focus on creating Fraud Detection Application to detect fraudulent credit card transactions. Thus, consumers and credit card companies are not paying for items that they did not purchase. According to Macaraeg (2019), the predicted worldwide non-cash transition growth from 2016 to 2020 is 12.7%. The increase in non-cash transactions leads to an increase in fraudulent transactions (Macaraeg, 2019). Even with EMV smart chips being implemented, the amount of money lost from credit card fraud is still very high. Therefore, implemented fraud detection (using data mining) is important. I also a 50 pages of fraud research (by myself) that can be found [ here](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/Report.pdf).

![alt](https://github.com/jackyhuynh/realtimeFraudDetectionModels-app/blob/main/src/picture/operationDiagram.PNG)

My application will be build from various data minning and model prediction methods. The combination of them will increase the change to prevent fraud detection. The disadvantage of this is the response time to end-users as many layer of detection will add more execution time to application (O(log(n))).
Please click [here](https://github.com/jackyhuynh/salePredictionModels-dataMining/blob/main/src/Markdown-WholeSale.pdf) for the full statistic and prediction. 

### Technology
* Business Analyst
* Machine Learning
* Data Mining
* Data Visualization
* AI

### Algorithm & Methods
* Data Exploration: Explore min, max, mean, standard deviation, correlation, and else using describe function
* Data Transformation: There is a lot of variation in the magnitude of the original data (org_data). To bring all the features to the same magnitude, standardize the features
* Principal Component Analysis (PCA)
* Eigen Vector
* Hopskin Statistic
* Elbow method (cluster analysis)
* Shilhouette method (cluster analysis)
* Representative-based clustering methods
* Hierarchal clustering methods
* Density-based clustering 

## Getting Started
These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Data
Please download data at [kaggle.com](https://www.kaggle.com/truchuynh87/wholesalecustomersdata) first.

### Prerequisites
What things you need to install the software and how to install them:
- R CRAN Project: R is a free software environment for statistical computing and graphics. It compiles and runs on a wide variety of UNIX platforms, Windows and MacOS
- RStudio IDE: RStudio is an integrated development environment (IDE) for R. It includes a console, syntax-highlighting editor that supports direct code execution, as well as tools for plotting, history, debugging and workspace management. Click here to see more RStudio features. RStudio is available in open source and commercial editions and runs on the desktop (Windows, Mac, and Linux) or in a browser connected to RStudio Server or RStudio Server Pro (Debian/Ubuntu, Red Hat/CentOS, and SUSE Linux)

### Installing

A step by step series of examples that tell you how to get a development enviroment running:
* [Install R](https://www.r-project.org/) - If you haven't downloaded and installed R, here's how to get started.
* [R Studio IDE](https://rstudio.com/products/rstudio/#:~:text=RStudio%20Take%20control%20of%20your%20R%20code%20RStudio,tools%20for%20plotting,%20history,%20debugging%20and%20workspace%20management.) - After that choose R Studio Desktop, and the free version (unless you have the Pro install). R free version is pretty good IDE.


## Running the tests

Explain how to run the automated tests for this system:
- Start R Studio.
- Create new a project.
- Copy the data and markdown file (.rmd) into the source file. For examaple:
```
~/salePredictionSystem/markdown.rmd
~/salePredictionSystem/WholesaleCustomersData.csv
```

- you can store the WholesaleCustomersData.csv in the same folder, but it is recommeded to store in a data as below (coding standard):
```
~/salePredictionSystem/data/WholesaleCustomersData.csv
```

- Make sure to change the import code on top if you want move your data anywhere. Depend on where you download the code. Your path will definately be different from mine. Please replace the path below with your own path:
```
WholesaleData <- read.csv("~/R/DataMining/WholeSale/data/WholesaleCustomersData.csv")
# path:("~/R/DataMining/WholeSale/data/WholesaleCustomersData.csv")
```

- Please take a quick view of [import data in R](https://support.rstudio.com/hc/en-us/articles/218611977-Importing-Data-with-RStudio?mobile_site=true) if you fail to change the import code.

### Data Visualization:

Using cluster analysis, we can find out potential customers' interest. Based on that group we can figure out what is our incoming inventories should be.

![alt](https://github.com/jackyhuynh/salePredictionModels-dataMining/blob/main/src/picture/2.PNG)


## Deployment
This can be deployed to any data base system for inventory prediction. Please note the application will work with any bigger or smaller data set as long as it follow the design pattern of this data set. Which mean the two nominal attributes must stay at the same names. 
- (7) CHANNEL: customers Channel — Horeca (Hotel/Restaurant/Caf??) or Retail channel (Nominal) 
- (8) REGION: customers Region of Lisbon, Oporto or Other (Nominal)
More continous attributes can just be add to the application, and it should work fine. Please refer to my research paper for better understanding. [Full research paper can be found here](https://github.com/jackyhuynh/salePredictionModels-dataMining/blob/main/src/Markdown-WholeSale.pdf).

I will not guarantee that this aplication will work "Big data set". If you are interested in "Big(or Large) data set" please join here for [an argue](https://www.researchgate.net/post/How-much-data-is-considered-to-be-small-data-Large-data-in-data-mining) on what data set is consider a large data set in data mining.

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
* **Purdue FortWayne University** - *Dataset* - Dataset was provide by Purdue FortWayne University CIS Department, and upload to kaggle.com by me.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

