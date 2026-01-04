# Credit Risk Repository
This repository contains analyses related to credit risk (ACL/CECL, Loss-Given-Default, Probability of Default, etc.).

The readme contains a short description of each analysis under its relevant sub-heading.


# Loss-Given-Default (LGD)

1. Comparison of Zero/One Inflated Beta Regression vs. Beta Regression with squished endpoints.
LGDs are a percent of the defaulted balance and are therefore bounded between 0% and 100%.
Modeling with linear regression will quickly lead to predicted LGDs that are < 0% or > 100%.
We also are generally interested in LGD behaviour between 0% and 100% so Logistic Regression, or a similar classifier, doens't work as well.
LGDs are commonly 0% and 100%, which makes us unable to use Beta Regression on its own.
There are 2 commonly suggested approaches to modeling fractions: use ZOIB or squish the endpoints so that the 0% values are not quite 0%.<br>This analysis simulates data, then compares the accuracy and interpretibility of both methods.<br>Analysis started on: 1/1/2026
