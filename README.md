# Neural_Network_Charity_Analysis

## Overview of Analysis
The purpose of this analysis was to determine whether applicants to Alphabet Soup were promising candidates and ultimately had a good chance to make the most of the organization's donation.

## Results

### Data Preprocessing
- The target for the model is the "IS_SUCCESSFUL" column.
- The features used for analysis are "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT".
- Both "EIN" and "NAME" were removed at the beginning of the process as they are unique and would not be of value to the analysis.

![image1_droppedColumns](/image1_droppedColumns.png)

### Compiling, Training, and Evaluating the Model
- The initial model that was prepared used two hidden layers (one with 80 neurons, another with 30 neurons) and the relu function. Eighty neurons were chosen as 
- The first model peaked at ~53% accuracy.
- Three ensuing iterations were tested after being adjusted as follows:
   * Two layers (each with 80 neurons) and each activated with the relu function
   * Two layers (one with 80 neurons, another with 30 neurons) and each activated with the sigmoid function
   * One layer with 80 neurons activated with the relu function

## Summary
Unfortunately, none of the model versions were able to approach the desired 75% threshold. Each hovered around the 53% mark, but there are countless additional alterations that could potentially improve its performance. Hidden layers could be added and removed, neurons could be increased and decreased, and activation functions could be rotated in pursuit of the best possible result. Another option would be to adjust the preprocessing actions taken on the data and rethink the size/breakdown of the bins used for application type/classification.
