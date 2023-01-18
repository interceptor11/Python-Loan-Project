# Python-Loan-Project

Introduction - Loans dataset aims to identify variables which indicate if a
person is likely to default, which can be used for identifying the risky loan
applicants to avoid any financial loss to the company.
Dataset Description - It contains the complete loan data for all loans
issued through the time period 2007 to 2011.
Data Dictionary -
1.annual_inc - The self-reported annual income provided by the borrower
during registration.
2.dti - A ratio calculated using the borrower’s total monthly debt payments on
the total debt obligations, excluding mortgage and the requested LC loan,
divided by the borrower’s self-reported monthly income.
3.emp_length -Employment length in years. Possible values are between 0 and
10 where 0 means less than one year and 10 means ten or more years.
4.funded_amnt - The total amount committed to that loan at that point in
time.
5.funded_amnt_inv -The total amount committed by investors for that loan at
that point in time.
6.grade - LC assigned loan grade
7.id - A unique LC assigned ID for the loan listing.
8.installment - The monthly payment owed by the borrower if the loan
originates.
9.int_rate - Interest Rate on the loan
10.last_pymnt_amnt-Last total payment amount received
11.last_pymnt_d -Last month payment was received
12.loan_amnt -The listed amount of the loan applied for by the borrower. If at
some point in time, the credit department reduces the loan amount, then it
will be reflected in this value.
13.loan_status - Current status of the loan
14.member_id -A unique LC assigned Id for the borrower member.
15.purpose - A category provided by the borrower for the loan request.
16.term -The number of payments on the loan. Values are in months and can
be either 36 or 60.
17.total_acc -The total number of credit lines currently in the borrower's credit
file
18.total_pymnt -Payments received to date for total amount funded
19.total_pymnt_inv -Payments received to date for portion of total amount
funded by investors
20.total_rec_int -Interest received to date
Questions -
1. Import the dataset and understand it.
2. List down the number of rows and columns.
3. ‘Int_rate’ column is character type. With the help of lambda function
convert into float type.
4. Check the datatype of each column.
5. Cleaning the dataset- Remove the columns having complete NaN value in
the entire dataset.
6. Write the code to find the value counts of the ‘loan_status’ category
column and filter only the ‘fully paid’ and ‘charged off’ categories.
7. Filter the ‘Emp_Len’ column to extract the numerical value from the
string.
Hint - Emp_len : < 1year, 2 years , 3 years as 1 , 2, 3 so on.
8. Using the Lambda function, remove the month from the ‘term’ column
such that ‘36 months’, ‘60 months’ appear as 36 and 60 respectively.
9. Create a new column as risky_loan_applicant by comparing loan_amnt
and funded_amnt with the following criteria -
If loan_amnt is less than equals to funded_amnt set it as ‘0’ else set it as
‘1’.
10. Using the bar plot visualize the loan_status column against categorical
column grade, term, verification_status . Write the observation from
each graph.
11.Using a user defined function convert the ‘emp_len’ column into
categorical column as follows -
If emp_len is less than equals to 1 then recode as ‘fresher’.
If emp_len is greater than 1 and less than 3 then recode as ‘junior’.
If emp_len is greater than 3 and less than 7 then recode as ‘senior’
If emp_len is greater than 7 then recode as ‘expert’.
12.Find the sum of ‘loan_amnt’ for each grade and display the distribution
of ‘loan_amnt’ using a pie plot.
