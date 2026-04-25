# Data Dictionary

This document describes the columns used in the Lending Club loan dataset after preprocessing.

| Column Name            | Description                                                                 |
|:-----------------------|:----------------------------------------------------------------------------|
| `loan_status`          | Current status of the loan (e.g., Fully Paid, Charged Off).                 |
| `loan_amnt`            | The listed amount of the loan applied for by the borrower.                  |
| `term`                 | The number of payments on the loan. Values are in months.                   |
| `int_rate`             | Interest Rate on the loan.                                                  |
| `installment`          | The monthly payment owed by the borrower.                                   |
| `grade`                | LC assigned loan grade.                                                     |
| `emp_length`           | Employment length in years.                                                 |
| `home_ownership`       | The home ownership status provided by the borrower during registration.     |
| `annual_inc`           | The self-reported annual income provided by the borrower during registration.|
| `verification_status`  | Indicates if income was verified by LC, not verified, or source verified.   |
| `purpose`              | A category provided by the borrower for the loan request.                   |
| `addr_state`           | The state provided by the borrower in the loan application.                 |
| `dti`                  | A ratio calculated using the borrower’s total monthly debt payments.        |
| `delinq_2yrs`          | The number of 30+ days past-due incidences of delinquency in the past 2 years.|
| `fico_range_low`       | The lower end of the borrower’s FICO range at loan origination.             |
| `fico_range_high`      | The upper end of the borrower’s FICO range at loan origination.             |
| `inq_last_6mths`       | The number of inquiries by creditors in the past 6 months.                  |
| `open_acc`             | The number of open credit lines in the borrower's credit file.              |
| `pub_rec`              | Number of derogatory public records.                                        |
| `pub_rec_bankruptcies` | Number of public record bankruptcies.                                       |
| `revol_bal`            | Total credit revolving balance.                                             |
| `revol_util`           | Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.|
| `total_acc`            | The total number of credit lines currently in the borrower's credit file.   |
| `tot_cur_bal`          | Total current balance of all accounts.                                      |
| `tot_hi_cred_lim`      | Total high credit/credit limit.                                             |
| `issue_d`              | The date which the loan was funded.                                         |
| `earliest_cr_line`     | The date the borrower's earliest reported credit line was opened.           |
| `acc_now_delinq`       | The number of accounts on which the borrower is now delinquent.             |
| `mort_acc`             | Number of mortgage accounts.                                                |
| `loan_default`         | Target variable: 1 if loan is defaulted/charged off/late, 0 otherwise.      |
| `issue_year`           | Year the loan was issued. Derived from `issue_d`.                           |
| `issue_month`          | Month the loan was issued. Derived from `issue_d`.                          |
| `credit_age_months`    | Age of borrower's credit history in months at time of loan issue.           |
| `emp_length_n`         | Numeric representation of employment length (years).                        |
| `term_n`               | Numeric representation of loan term (months).                               |
| `loan_to_income`       | Ratio of loan amount to annual income.                                      |
| `fico_avg`             | Average of `fico_range_low` and `fico_range_high`.                          |
| `delinq_flag`          | Flag: 1 if `delinq_2yrs > 0`, 0 otherwise.                                  |
| `high_risk_flag`       | Flag: 1 if `dti > 30` or `fico_avg < 650`, 0 otherwise.                     |

