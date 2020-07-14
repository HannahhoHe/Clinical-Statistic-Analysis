
# Data Format
The first column is for sample ID (slide ID, patient ID); the second column for "time" of overall survival (OS) or relapse (PFS); the third column is whether the patient has deceased (=1) or relapsed (=1); and all other features should be put from column four to the end.    
- This script starts with predictors as regression and convert them to categorical
- In some cases, if features are collinear, a penalizer in the CoxPHFitter is needed (line 23)
- Be sure to remove samples with unknown os/pfs in the third column
- Be sure not to include any features with NA values
