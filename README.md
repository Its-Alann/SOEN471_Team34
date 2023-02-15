# SOEN471 - Sofvie Project 8 - Team 34

Training programs are crucial in many workplace environments to ensure that employees have up-to-date skills and knowledge about certain procedures. Safety training in particular greatly prevents the risk of an incident occurring by increasing awareness in the event of a possible hazard. 

Sofvie [1] is a company that focuses on efficiency and employee safety by adopting a proactive approach to employee training. Our goal with this project is to evaluate the quality of training procedures by looking at training completion rates with big data driven methods.

Our dataset has been provided to us in the form of various schemas and template SQL scripts. By running SQL queries we determined that it contains the information of **2001** employees, **2** different training types that branch out into **776** unique training codes, and a pairing of **33,115** training amongst employees. Our **dataset features** include:
- Employee table 
  - Employee number [varchar]
  - Employee position id [int]
  - Start/End date [datetime]
- Employee training table
  - Training type [int]
  - Training code [int]
  - Trainings completed by the employee [int]
- Person
  - Generation ['Boomer', 'Gen X', 'Millenial', 'Gen Z']
  - Gender [varchar]

Due to receiving our dataset on quite short notice (02/13/2023), more features will come to light as we make progress. We may eventually ask Sofvie to provide us with other relevant features such as ‘employee pay grade’ or ‘training duration’ that could play a role in employee willingness to complete a training.

Based on our dataset, we will seek to answer the following **research questions**:

1. What factors increase the likelihood of an employee having higher training completion rates?

2. What are the features in common for employees with different completion rates?

3. What are the common factors in training with high completion rates versus those with low completion rates?

To better understand our data, we will begin by graphing two histograms on training completion rates in regards to both employees and trainings. This will show us if we're working with two distinct clusters such as high and low completion rates to use as our labels.   

We will then approach our research questions both from a **clustering and a supervised classification model** point of view. 

With clustering, we will use kmeans and hierarchical clustering algorithms to better define the cut-off point of both groups and analyze their common factors. From both the employee and the training perspective, we hope to gain insight on common features of motivated employees as well as common characteristics of trainings that resonate well with employees.

With supervised classification, we will use random forests and deep neural networks to predict whether an employee will have high or low completion rate based on features that have a greater impact. We may also explore supervised regression to predict the completion rate of an employee based on past training data and employee information.


References:

[1] https://sofvie.com

Word count: 459

## Team Members 
- Daria Denejkina
- AmirHossein Zamani
- Ali Sabaghpourfard
- Alan Matthew Vadlakunta
