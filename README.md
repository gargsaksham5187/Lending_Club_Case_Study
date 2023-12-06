# Lending Club Case Study

## <font color='red'> Loan Approval Risk Analysis </font>

# Case Study Goals:
   * Data understanding  (10%)
   * Data Cleaning and Manipulation (20%)
   * Data analysis (40%, (Univariate and segmented univariate analysis,Business/data driven metrics, Appropriate plots)
   * Presentation and Recommendations (20%)
   * Conciseness and readability of the code (10%)   


#### Group members
- Saksham Gupta
- Sreehari Varma


### Assignment Brief:
You work for a consumer finance company **Lending Club** which specialises in lending various types of loans to urban customers. This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. When the company receives a loan application, the company has to **make a decision for loan approval based on the applicant’s profile.**
When a person applies for a loan, there are two types of decisions that could be taken by the company:

**1. Loan accepted:** If the company approves the loan, there are 3 possible scenarios described below:

**Fully paid:** Applicant has fully paid the loan (the principal and the interest rate)

**Current:** Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

**Charged-off:** Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

**2. Loan rejected:** The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)



### Business Objectives:
Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). The credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders.


Objective is to **identify the risky loan applicants at the time of loan application** so that such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, **to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.**  The company can utilise this knowledge for its portfolio and risk assessment. And thus minimise the risk of losing money while lending to customers.


## Conclusion:

#### Major variables to consider for loan prediction:

        1. Loan Purpose
        2. Employment Length
        3. Interest Rate
        4. Annual Income
        5. Grade & Sub-grade
        6. Term
        7. Address State
        
### More Insights -

### Loan Purpose:
##### Charged Off Rate is high for loan purpose:

        1. small_business    = 26.27%
        2. renewable_energy  = 18.81%
        3. educational       = 17.03%
        

### Employment Length: 
##### Charged Off Rate is high for employment length:
        
        1.  0 year (< 1 year)
        2.  1 year
##### We see that the Charged Off rate increases for peopple with less employment length.

### Interest Rate:
##### Charged Off Rate is high  for interest rate:
        
        1. 20-25   = 34.44%
        2. 15-20   = 23.51%
###### As the Interest Rate increases, Charge Off Rate Increases


### Annual Income:
##### Charged Off Rate is high for Annual Income:
        
        1. 0-20000       = 19.93%
        2. 20000-40000   = 17.43%
        3. 40000-60000   = 14.90%
##### So, as the Anual Income decreases, Charge Off Rate Increases


### Grade & Sub-grade:
##### Most of the Charged off applicants belong to Grade B, C and D.
##### Of the Grade B, C and D, most of the Charged off applicants belong to Sub Grades:
        
        1. Grade B => B3, B5, B4
        2. Grade C => C3, C4, C5
        3. Grade D => D3, D4, D5

##### Also as the Grade increases, Charged Off Rate increases. Top Order:
        
        1. G
        2. F
        3. E
        4. D
        5. C
        6. B
        7. A


### Term:
##### Charge Off Rate increases as the Term increases.


### Address State:
##### Charged Off Rate is high for Address State:
        
        1. NE (Nebraska)     = 60.00%
        2. NV (Nevada)       = 21.75%
        3. SD (South Dakota) = 18.75%
        4. AK (Alaska)       = 17.72%
        5. FL (Florida)      = 17.54%

        *NE (Nebraska) has a total of 5 loans out of which 3 were charged-off.
