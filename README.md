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

**Model**: 
1. Logistic Regression
    - Accuracy : 85 %
    - AUC : 56 %
2. Random Forest
    - Accuracy : 89 %
    - AUC : 71 %

**Insights** : The most influencing factors
1. CustServCalls -> number of calls into customer service
2. DayMins  -> average daytime minutes per month
