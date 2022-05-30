# Module 14 Challenge
 
## Purpose
The goal of this project is to enhance the company's current machine learning trading bot by examining current trading signals to adapt new data and keep competition in the marketplace.  This will be done by using pandas to create dataframes to train and test data splits as well as using plot and hvplot to visualize said data.  We will be directly comparing cumulative performance of Actual returns vs Strategy returns and StandardScaler to preprocess the data to further accuracy.  The two classifiers being used to enhance the models are SVC and LogisticRegression from the Sklearn library.  


## Trading Algorithims

### Baseline
* Short Window of 4
* Long Window of 100
* Date Offset of 3 Months
* Training Days of 3 not including Date Offset
* Buy stock long
    * precision: .63
    * recall: 1.0
    * f1-score: .77
* Sell stock short
    * precision: 1.00
    * recall: .06
    * f1-score: .12
    
### Size-adjusted (changed size of training set from 3 to 6 months)
* Short Window of 4
* Long Window of 100
* Date Offset of 6 Months
* Training Days of 3 not including Date Offset
* Buy stock long
    * precision: .58
    * recall: .89
    * f1-score: .70
* Sell stock short
    * precision: .59
    * recall: .20
    * f1-score: .29
    
### Size adjusted & SMA adjusted
* Short Window of 10
* Long Window of 150
* Date Offset of 6 Months
* Training Days of 3 not including Date Offset
* Buy stock long
    * precision: .56
    * recall: .93
    * f1-score: .70
* Sell stock short
    * precision: .64
    * recall: .15
    * f1-score: .24


