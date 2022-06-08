# Lending Club
> This is an analysis on Lending Club, to provide insight on loan data to minimize the loss on new loans.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.

    The data contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

- What is the background of your project?

    When a person applies for a loan, there are two types of decisions that could be taken by the company:

    Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

    Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

    Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

    Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

    Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
- What is the business probem that your project is trying to solve?

    This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

    Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

    If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

    In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 

    To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

- What is the dataset that is being used?

    [dataset](data/loan.csv)

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions

We can detect bad loans,
- Higher amount of loan were given to people, with less DTI.
- Similarly, Higher amount of loan given to people with lower annual income bracket.
- Grade G, is the grade with highest interest rate but we can see that it has been loaned to
people who are not verified, where around 42% loan gets charged off.
- Don’t provide loan for small_buisness unless they get verified. There is 42% probability that
loan get charged off if it is provided for small business without verification
- Highest bracket of interest Rate were given to “Not Verified” borrower, which can be prevented from charged off.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Numpy
- Pandas
- Seaborn/Matplotlib
- Python

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->



## Contact
Created by [[@har2008preet](https://github.com/har2008preet) & [@sidshrivastav](https://github.com/sidshrivastav)] - feel free to contact us!
