# Trading Signals (Algorithms) with Machine Learning


**Background:**

As a Financial Advisor at one of the major Financial Institution, I have analyzed the Daily Closing Prices of Stock: "OHLCV". Where, I have calculated the Actual Returns of the stock for each day price movements by applying "Change in %" formula in daily closing prices of stock. 

In order to create: **"Trading Algorithm - Machine Learning Model"** I have considered the "Actual Returns" value as a Signal for Buying & Selling the Stock. 

Where, I have defined the following conditions:

If, the Actual Returns >= 0 then system returns Signal value as: 1 (Where, 1 means: **BUY**)

If, the Actual Returns < 0 then system returns Signal value as: -1 (Where, -1 means: **SELL**)


I have tested various Models to get the accurate predictions, following are the models I have used with their Performance Summary including "Classification Report" & "Cumulative Return Chart":




**TRIAL 1: MODEL PERFORMANCE SUMMARY:**

Following are the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 04 Days & Long Window = 100 Days

**Model:**
SVC Classifier

**Classification Report:**


![Classification Report - Original Data](https://user-images.githubusercontent.com/86034323/135793798-b3f85bdc-195a-40a3-9055-b2c170a7f0d2.png)


**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![Model Performance - Original](https://user-images.githubusercontent.com/86034323/135791410-629e2fe1-d94f-43de-92cb-a3ba9cdb0562.png)


**TRIAL 2: MODEL PERFORMANCE SUMMARY:**

Following are the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 04 Days & Long Window = 100 Days

**Model:**
AdaBooster Classifier

**Classification Report:**


![Classification Report - AdaBoosterClassifier](https://user-images.githubusercontent.com/86034323/135794139-91b2cbe4-afb5-45a4-a49a-7bef53bcd634.png)


**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![Model Performance - AdaBoostClassifier](https://user-images.githubusercontent.com/86034323/135794179-f2a902ed-f948-4445-82f9-cd352563abfa.png)



**TRIAL 3: MODEL PERFORMANCE SUMMARY:**

Following are the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 07 Days & Long Window = 60 Days

**Model:**
SVC Classifier

**Classification Report:**


![Classification Report - SVC (SMA - 07, 60)](https://user-images.githubusercontent.com/86034323/135794354-6cef0a15-d364-40f5-a757-b43c19553184.png)


**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![Model Performance - SVC (SMA - 07, 60)](https://user-images.githubusercontent.com/86034323/135794383-9af3bc39-8703-488f-9f3e-edfe8060d374.png)



**TRIAL 4: MODEL PERFORMANCE SUMMARY:**

Following are the input parameters:

**Simple Moving Averages (SMA):**
Short Window = 07 Days & Long Window = 60 Days

**Model:**
AdaBooster Classifier

**Classification Report:**

![Classification Report - AdaBoosterClassifier (SMA - 07, 60)](https://user-images.githubusercontent.com/86034323/135794478-3d1e0219-e38c-4319-a7cd-ca453bbe9a29.png)


**Cumulative Return Plot: Actual Returns vs. Strategy Returns**


![Model Performance - AdaBoostClassifier (SMA - 07, 60)](https://user-images.githubusercontent.com/86034323/135794509-433614d3-2485-46a0-a99b-e260b77f87c3.png)



**FINDINGS:**
After Considering: Classification Reports & Cumulative Returns Visual Charts of all 4 Trials, it looks like that TRIAL 4 after applying "AdaBooster Classifier" with this input parameter of "SMA Readings": Short-Window = 07 Days & Long Window = 60 Days are the most appropriate ones to train this model. 

Since, Actual & Strategy Returns are quite close to each other therefore TRIAL 4 Model is the most fitted model on this dataset.
