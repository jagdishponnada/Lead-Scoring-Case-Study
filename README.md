# Lead-Scoring-Case-Study

## Background
An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses.    The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%.    Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone.

## Objectives
We aim is to build a model wherein we need to assign a lead score  between 0 and 100  to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance. 

##  Data
The data provided (leads dataset) are from the past with around 9000 data points. This dataset consists of various attributes such as Lead Source, Total Time Spent on Website, Total Visits, Last Activity, etc. which may or may not be useful in ultimately deciding whether a lead will be converted or not. The target variable, in this case, is the column ‘Converted’ which tells whether a past lead was converted or not wherein 1 means it was converted and 0 means it wasn’t converted.

## Tech Stack
- Language - Python 3.7 
- Libraris 
  - Numpy and pandas for Data preprocessing
  - Seaborn and Matplotlib for Data visualisation
  - Sklearn (Logistic Regression) for Modelling.


## Results 
We computed the sensitivity , accuracy and specificity 
  - Accuracy: 0.77
  - Sensitivity:0.82
  - Specificity:0.75

## Recommendations
The top 3 variables to be focused are Lead Origin_Lead Form, Last Activity_Had a Phone conversation, Lead Source_chat.  All the three variables signify the Lead’s interest towards X education. 

- Lead Origin_Lead Form:
If the Lead Origin is Lead form which is kind of filling form, then there is more chance that lead will join the online course in X Education since leads are taking some steps towards joining the course. 

- Last Activity_Had a Phone conversation:
By tracking the leads activity, it’s found that  ‘Had a Phone conversation’ activity is the significant activity as per the final model to increase the probability of lead conversion. It’s clear that leads who had a phone conversion are joining the course mostly. Hence, X Education train the sales team such that the conversion rate will be increased after the phone conversation.  

- Lead Source_chat:
Among the various sources of lead such as search engines, chat, direct traffic, references, social medias, etc., chat gains the noticeable attention to the leads which makes them to join the online course. Hence, X education needs to concentrate on Olark chart and Live charts to get more customers to be converted into potential leads.
