# Product-Failure-prediction
1. Product Failure probability using Logistic Regression.
2. Feature Engineering involved creating features based on the following Hypothesis testing
   * **Null Hypothesis** : Mean failure rate of missing values = Mean failure rate of values not missing

   * **Alternate Hypothesis** : Mean failure rate of missing values $\neq$ Mean failure rate of values not missing.

   * **Hence it will be a two tailed test.**

   * We will take level of significance, that is, the probability of making a Type 1 error to be 0.05.

   * **Rejection rule** : Rejection null hypothesis if p value $\le$ level of significance.
   * Calculated p-value and zscore using scipy.stats library.
   * Results
     * - The difference between mean failure rate of missing values and mean failure rate of values not missing is statistically significant only for measurement_3 and measurement_5.

      - So, the null hypothesis for measurement_3 and measurement_5 will be rejected while for other features we cannot reject null hypothesis.

      - We will create new feature for measurement_3 and measurement_5 giving information abot values missing or not missing.

      - While for other features just impute missing values.
  3. Got a mean cross validation roc_auc_score of 0.58 on 5 folds.
  

