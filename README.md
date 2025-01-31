# classification-churn

**Problem** : Classificaton

**Data** : 
1.  Churn : 1 if customer cancelled service, 0 if 
    - 0 : 2850
    - 1 : 483
2.  AccountWeeks : number of weeks customer has had active account
3.  ContractRenewal : 1 if customer recently renewed contract, 0 if not
4.  DataPlan : 1 if customer has data plan, 0 if not
5.  DataUsage : gigabytes of monthly data usage
6.  CustServCalls : number of calls into customer service
7.  DayMins : average daytime minutes per month
8.  DayCalls : average number of daytime calls
9.  MonthlyCharge : average monthly bill 
10. OverageFee : largest overage fee in last 12 months

**Feature Importance** : calculate the importance score for each feature
1. Logistic Regression 
    - ContractRenewal : -0.59
    - DataPlan : -0.504
    - CustServCalls : 0.67
    - DayMins : 0.54
2. Random Forest 
    - CustServCalls : 0.14
    - DayMins : 0.20
    - MonthlyCharge : 0.17
3. Xgboost
    - ContractRenewal : 0.16
    - DataPlan : 0.45
    - CustServCalls : 0.13
4. KNN
    - ContractRenewal : 0.03
    - CustServCalls : 0.04
    - DayMins : 0.05
    - MonthlyCharge : 0.03

**SMOTE (Oversampling)**: balancing classes by creating synthetic samples from the minority class (churn = 1)
- 0 : 2281
- 1 : 2281

**Model**: 
1. Logistic Regression
    - Accuracy : 75 %
    - AUC : 74 %
2. Random Forest
    - Accuracy : 88 %
    - AUC : 80 %
3. Xgboost
    - Accuracy : 88 %
    - AUC : 81 %

**Insights** : The most influencing factors
1. CustServCalls -> number of calls into customer service
2. DayMins  -> average daytime minutes per month
3. ContractRenewal -> 1 if customer recently renewed contract, 0 if not
