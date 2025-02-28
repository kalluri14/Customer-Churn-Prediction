# Customer-Churn-Prediction

## Step1: load your dataset
We have used the Telecom_churn dataset from kaggle

## Step2: Data preprocessing
    - Data (There are total 20 columns, 7043 entries from 0 to 7042)
    - Check for data type of each column, TotalCharges was originally object but then we convert it to float type
    - check for missing and null values (all are non null, so total null values : 0)
    - check for duplicates(There are no duplicates)
    - check for categorical data(other than 3 columns(SeniorCitizen, Tenure, TotalCharges and MonthlyCharges) all the other are categorical columns)

    - Summary Stats of numeric columns:
        - SeniorCitizen: It is binary(Senior : 0 and Not Senior: 1) only 0.16 that is 16% of citizens are senior citizens
        - Tenure: On an average the no.of years worked are 32(mean), where as half of the persons tenure is <= 29 since meadian (50%) = 29, max no.of years worked = 72, min = 0
        - MonthlyCharges: Average monthly bill is 64$ and mini or chepest plan is 18$ and the costliest , highest is 118$, with half of the customers paying $70 or less
        - TotalCharges: Average Total Charge is 2279$ and mini charge starts from O to max charge 8684 $, half of the customers paying $1394 or less

    - Check for distributions:
        - we divide our data into mainly 3 sets 
            - Gender, partner, Dependents - personal attribute
            - "PhoneService", "MultipleLines", "InternetService", "OnlineSecurity", "OnlineBackup"   "DeviceProtection", "TechSupport", "StreamingTV", "StreamingMovies" - services attribute
            - "Contract", "PaperlessBilling", "PaymentMethod", "Churn" - Contract and Payment Attributes

    - Analysis of Categorical Visualizations:
        - The personal attributes seem to have equal distribution except for the dependents, almost 50% people have no dependents
        - Phone service is almost universal, but multiple lines aren’t as common.
        - Fiber optic is the dominant internet service.
        - Security, backup, and tech support services are underutilized.
        - Streaming services are used by a large number of customers, but not everyone opts for them.
        - A segment of customers doesn’t use internet-based services at all.
        - Month to month services are mostly availed indicating customers prefer short-term flexibility over long-term commitments.
        - paperless billing is more
        - payments made via electronic check are more compared to other payment methods which are equally distributed
        
    - Currently there are 5174 customers who did not churn and almost 26.5% customers(1869) churned.

    - Month-to-Month contract users churn the most, while One-Year and Two-Year contracts have significantly lower churn rates.
    - Customers with Paperless Billing have a higher churn rate than those receiving paper bills.
    - Electronic Check users have the highest churn, while automatic payment methods (Credit Card & Bank Transfer) show the lowest churn.

## Step3: Running Statistical Testing

    - To prove with statistical confidence that the features are having affect on our target label(Churn)
    - we first define our null and alternative hypothesis
    - perform chisquare test since we are dealing with categorical data
    - we reject or accept the null hypo based on the p-value we get from our test.

## Step4: Feature Engineering

    - Encoding categorical columns
    - scaling numerical columns
    
## Step5; Feature Selection

    - Drop low importance features, check correlation with churn






    








    