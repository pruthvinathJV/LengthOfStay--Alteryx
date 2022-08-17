# LengthOfStay--Alteryx
Predicting Length of Hospital stay based on MediCare claims data using Alteryx workflow

Input Data files:
  Beneficiary Summary (2008 - 2010): 3 different files
    32 attributes
    ~ 115,000 observations
    
  Inpatient claims (2008-10):
    81 attributes
    ~66,000 observations
    
   Outpatient claims (2008-10):
    76 attributes
    ~790,000 observations
    
   HCC Lookup (tells about the riskines of each beneficiary): 199,315 observations
   
   
Workflow in Alteryx:

1. cleaned each data set of nulls, '?' etc.
2. done exploratory data analysis and prepared data sets by remvoing irrelevant attributes
3. run the t-tests and correlation tests
4. in approach 1, taken dependent variable as the continuous variable --> Linear Regression Model
5. in approach 2, converted the dependent variable into a categorical variable --> Random forest and Decision tree models
6. After training the data set, ran the model on test data (created 80:20 samples)
7. compared between different models
8. still the model can be improved
   
