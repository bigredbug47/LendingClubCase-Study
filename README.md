# LendingClubCase-Study
The Lending Club Case study of Upgrad &amp; IIITB | Global Program in Machine Learning &amp; AI

<hr>
<br>
<h1>Business Understanding</h1>

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

<h1>Business Objectives</h1>

<li>This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. </li>

<li>Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.</li> 

<li>If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.</li>

<li><b>In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment</b></li>

<li>To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).
</li>

<hr>
<br>

<h1>Evaluation Rubric</h1>

<table>
    <tr>
        <th style="text-align:center">Criteria</th>
        <th style="text-align:center">Meets expectations</th>
        <th style="text-align:center">Does not meet expectations</th>
    </tr>
    <tr>
        <td style="text-align:center"><b>Data Understanding (10%)</td>
        <td>
            <li>All data quality issues are correctly identified and reported.
            <li>Wherever required, the meanings of the variables are correctly interpreted and written either in the comments or text.
        </td>
        <td>
            <li>Data quality issues are overlooked or are not identified correctly such as outliers, missing values and other data quality issues.
            <li>The variables are interpreted incorrectly or the meaning of variables is not mentioned.
        </td>
    </tr>
    <tr>
        <td style="text-align:center"><b>Data Cleaning and Manipulation (20%)</td>
        <td>
            <li>Data quality issues are addressed in the right way (missing value imputation, outlier treatment and other kinds of data redundancies, etc.).
            <li>
            If applicable, data is converted to a suitable and convenient format to work with using the right methods.
            <li>
            Manipulation of strings and dates is done correctly wherever required.
        </td>
        <td>
            <li>
            Data quality issues are not addressed correctly.
            <li>
            The variables are not converted to an appropriate format for analysis.
            <li>
            String and date manipulation is not done correctly or is done using complex methods.
        </td>
    </tr>
    <tr>
        <td style="text-align:center"><b>Data Analysis (40%)</td>
        <td>
            <li>The right problem is solved which is coherent with the needs of the business. The analysis has a clear structure and the flow is easy to understand.
            <li>Univariate and segmented univariate analysis is done correctly and appropriate realistic assumptions are made wherever required. The analyses successfully identify at least the 5 important driver variables (i.e. variables which are strong indicators of default).
            <li>Business-driven, type-driven and data-driven metrics are created for the important variables and utilised for analysis. The explanation for creating the derived metrics is mentioned and is reasonable.
            <li>Bivariate analysis is performed correctly and is able to identify the important combinations of driver variables. The combinations of variables are chosen such that they make business or analytical sense. 
            <li>The most useful insights are explained correctly in the comments.
            <li>Appropriate plots are created to present the results of the analysis. The choice of plots for respective cases is correct. The plots should clearly present the relevant insights and should be easy to read. The axes and important data points are labelled correctly.
        </td>
        <td>
            <li>The analyses do not address the right problem or deviate from the business objectives. The analysis lacks a clear structure and is not easy to follow.
            <li>The univariate and bivariate analysis is not performed in sufficient detail and thus some crucial insights are missed out. The analyses are not able to identify enough important driver variables.
            <li>New metrics are not derived wherever appropriate. The explanation for creating the derived metrics is either not mentioned or the metrics are not reasonable. 
            <li>Derived metrics are not analysed correctly/are insufficiently utilised.
            <li>Important insights are not mentioned in the report or the Python file. Relevant plots are not created. The choice of plots is not ideal and the plots are either difficult to interpret or lack clarity or neatness. Relevant insights are not clearly presented by the plots. The axes and important data points are not labelled correctly/neatly. 
        </td>
    </tr>
    <tr>
        <td style="text-align:center"><b>Presentation and Recommendations (20%)</td>
        <td>
            <li>The presentation has a clear structure, is not too long, and explains the most important results concisely in simple language.
            <li>The recommendations to solve the problems are realistic, actionable and coherent with the analysis. 
            <li>The GitHub repository link contains a Python file, presentation file and a README.md file. README.md file should describe the project briefly.
            <li>If any assumptions are made, they are stated clearly.
        </td>
        <td>
            <li>The presentation lacks structure, is too long or does not put emphasis on the important observations. The language used is complicated for business people to understand.
            <li>The recommendations to solve the problems are either unrealistic, non-actionable or incoherent with the analysis.
            <li>The GitHub repository should not be private.  
            <li>The GitHub repository link which does not contain a Python file, presentation file and a README.md file.
            <li>README.md file which has no proper brief description of the project.
            <li>Contains unnecessary details or lacks the important ones.
            <li>Assumptions made, if any, are not stated clearly.
        </td>
    </tr>
    <tr>
        <td style="text-align:center"><b>Conciseness and readability of the code (10%)</td>
        <td>
            <li>The code is concise and syntactically correct. Wherever appropriate, built-in functions and standard libraries are used instead of writing long code (if-else statements, for loops, etc.).
            <li>Custom functions are used to perform repetitive tasks.
            <li>The code is readable with appropriately named variables and detailed comments are written wherever necessary.
        </td>
        <td>
            <li>Long and complex code used instead of shorter built-in functions.
            <li>Custom functions are not used to perform repetitive tasks resulting in the same piece of code being repeated multiple times.
            <li>Code readability is poor because of vaguely named variables or lack of comments wherever necessary.
        </td>
    </tr>
</table>