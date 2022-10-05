Note: The answers to these questions are relative and sometimes debatable.
The most important thing is to be able to make intelligent comparisons between models regarding their pros and cons.

1. Is it interpretable?
  - KNN: Somewhat
  - LogReg: Yes
  - CART: Yes
  - RF: Somewhat
  - NB: Somewhat
  - GB: Somewhat
2. Is it inherently multi-class?
  - KNN: Yes
  - LogReg: No
  - CART: Yes
  - RF: Yes
  - NB: Yes
  - GB: Yes
3. Is it scalable with large number of features (in terms of execution time and quality of results)?
  - Execution time:
    - KNN: No
    - LogReg: Yes
    - CART: Yes
    - RF: Yes
    - NB: Yes
    - GB: Yes
  - Quality:
    - KNN: No
    - LogReg: Yes, with regularization
    - CART: Somewhat
    - RF: Yes
    - NB: Yes
    - GB: Yes 
4. Is it scalable with large number of data points (in terms of execution time and quality of results)?
  - Execution time:
    - KNN: No
    - LogReg: Yes
    - CART: Somewhat
    - RF: Somewhat
    - NB: Yes
    - GB: Somewhat
  - Quality:
    - KNN: Yes
    - LogReg: Yes
    - CART: Yes
    - RF: Yes
    - NB: Yes
    - GB: Yes
5. Is it good with diverse (non-homogenous) set of features?
  - KNN: No
  - LogReg: No
  - CART: Yes
  - RF: Yes
  - NB: No
  - GB: Yes
