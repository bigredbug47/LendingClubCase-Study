# LendingClubCase-Study
>The Lending Club Case study of Upgrad &amp; IIITB | Global Program in Machine Learning &amp; AI <br>
> Based on the lending data of company, we analyze and exploit all factors that have strong relationship with the status of loans.


## Table of Contents
* [General Info](#general-information)
* [Dataset](#datasDet)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Contact](#contact)

## General Information

### <b>Business Understanding</b>

<p>You work for a <b>consumer finance company</b> which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two <b>types of risks</b> are associated with the bank’s decision:

<li>If the applicant is <b>likely to repay the loan</b>, then not approving the loan results in a <b>loss of business</b> to the company
<li>If the applicant is <b>not likely to repay the loan</b>, i.e. he/she is likely to default, then approving the loan may lead to a <b>financial loss</b> for the company </li>

<br>

<p>The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
<p>In this case study, you will use EDA to understand how <b>consumer attributes and loan attributes</b> influence the tendency of default.

<p>When a person applies for a loan, there are <b>two types of decisions</b> that could be taken by the company:
<li><b>Loan accepted:</b> If the company approves the loan, there are 3 possible scenarios described below:
    <ul>
        <li><b>Fully paid:</b> Applicant has fully paid the loan (the principal and the interest rate)
        <li><b>Current:</b> Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.
        <li><b>Charged-off:</b> Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 
    </ul>
</li>
<li>
<b>Loan rejected:</b> The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
</li>

<hr>
<br>

### <b>Business Objectives</b>

<li>This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. </li>

<li>Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.</li> 

<li>If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.</li>

<li><b>In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment</b></li>

<li>To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).
</li>

<hr>
<br>

## Dataset
<li>The sample of loan data for all loans issued through the time period 2007 to 2011.</li>

<hr>

## Conclusions
- The <b>total payment below 10000$</b> which has <b>high rate of default loans</b> can be considered as the threshold for business to apply in their rules-based procedure
- The business should draws some specific rules that target only <b>higher grades (A->C) to increases sales</b> or focus on <b>lower grades (D->G) to reduce risks</b>
- <b>Interest rate over 12%</b> is the point where business should put more efforts to validate and analyze the potential <b>risk of lending cases</b> to reduce the bad rate
- <b><5000$ in Principal Received to Date</b> is the package that <b>75% charged off cases</b> can not reached
- Most of lending cases have <b>Lending Purposes</b> come from <b>Debt, Credit Card, Car and Home Improvement</b>. 


## Technologies Used
- Python - Version 3.8.10 64-bit
- Pandas - Version 1.3.0
- Numpy - Version 1.21.0
- Seaborn - Version 0.12.1
- Matplotlib - Version 3.4.2


## Contact
Created by [@bigredbug47] - feel free to contact me!