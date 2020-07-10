# Flatiron Data Science Project 3: Machine Learning Classification
By: Bradley Ellisor and Gabe Arnold

## Primary Goals:
Use Machine Learning techniques to determine feature importance.

## Introduction
In this project, we use classification machine learning techniques to create inferences into feature importance for bank marketing campaigns. 

### Business Case
The data is related with direct marketing campaigns (phone calls) of a Portuguese banking institution. The classification goal is to predict if the client will subscribe a term deposit (variable y).

### About our Data
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

## Attribute Information:

* ### Bank client data:

Age (numeric)

Job : type of job (categorical: 'admin.', 'blue-collar', 'entrepreneur', 'housemaid', 'management', 'retired', 'self-employed', 'services', 'student', 'technician', 'unemployed', 'unknown')

Marital : marital status (categorical: 'divorced', 'married', 'single', 'unknown' ; note: 'divorced' means divorced or widowed)

Education (categorical: 'basic.4y', 'basic.6y', 'basic.9y', 'high.school', 'illiterate', 'professional.course', 'university.degree', 'unknown')

Default: has credit in default? (categorical: 'no', 'yes', 'unknown')

Housing: has housing loan? (categorical: 'no', 'yes', 'unknown')

Loan: has personal loan? (categorical: 'no', 'yes', 'unknown')

* ###  Related with the last contact of the current campaign:

Contact: contact communication type (categorical:'cellular','telephone')

Month: last contact month of year (categorical: 'jan', 'feb', 'mar',
…, 'nov', 'dec')

Dayofweek: last contact day of the week (categorical:
'mon','tue','wed','thu','fri')

Duration: last contact duration, in seconds (numeric). Important
note: this attribute highly affects the output target (e.g., if
duration=0 then y='no'). Yet, the duration is not known before a call
is performed. Also, after the end of the call y is obviously known.
Thus, this input should only be included for benchmark purposes and
should be discarded if the intention is to have a realistic
predictive model.


* ###  Other attributes:

Campaign: number of contacts performed during this campaign and for
this client (numeric, includes last contact)

Pdays: number of days that passed by after the client was last
contacted from a previous campaign (numeric; 999 means client was not
previously contacted)

Previous: number of contacts performed before this campaign and for
this client (numeric)

Poutcome: outcome of the previous marketing campaign (categorical:
'failure','nonexistent','success')

* ### Social and economic context attributes

Emp.var.rate: employment variation rate - quarterly indicator
(numeric)

Cons.price.idx: consumer price index - monthly indicator (numeric)

Cons.conf.idx: consumer confidence index - monthly indicator
(numeric)

Euribor3m: euribor 3 month rate - daily indicator (numeric)

Nr.employed: number of employees - quarterly indicator (numeric)

* ###  Output variable (desired target):

y - has the client subscribed a term deposit? (binary: 'yes', 'no')



## Methodology
## Steps

1. Import Libraries
2. Upload and Clean Dataset
3. EDA
4. Hypothesis Testing
5. Feature Engineering
6. Feature Selection
7. Model Creation and Selection
8. Model Tuning
9. Analysis & Conclusion



## Conclusion
Not surprisingly, our most important features came from the economy metrics category and bank relationship category. When we consider what a term deposit is,  this makes a lot of sense. Essentially a term deposit is the bank asking their clients to deposit a certain amount of cash for a fixed period of time in exchange for interest on the sum. These commonly range from 6 months to 2 years but can go as high as 10 years. People who are employed in a good economy are more likely to deposit cash into term deposits than people who need the cash to be as liquid as possible. 

Therefore, Banks should focus their marketing campaigns on clients who are gainfully employed in a good market. Today's market highly volatile so term deposits are not really an appropriate product to market and money will likely be a waste. Instead, banks can focus on developing strong relationships with their clients in times of need as past relationships are also a factor. 





