# coursera_salifort_capstone_project
This project is based on a fictional database proposed as part of the Google Advanced Data Analytics Professional Certificate program, which I completed on May 23, 2024.

Salifort Motors Employee Turnover Analysis

Overview

This project analyzes the employee turnover at Salifort Motors, an imaginary company. The goal is to understand the reasons behind the high turnover rate and to develop a predictive model to help prevent undesirable resignations. This project is based on a fictitious dataset provided as part of the “Google Advanced Data Analytics Professional Certificate” program.

Certificate

You can view the certificate for the completed program here: https://coursera.org/share/703bf292ebc8f7389a2aee192b635606.

Objectives

1.	Conduct an exploratory data analysis (EDA) to identify groups and potential causes for the high turnover rate.
2.	Develop a classification model to predict with significant probability whether an employee is likely to resign. This model will help identify the most critical factors influencing employee turnover.

Project Plan

1.	Preparation: Downloading the dataset and necessary imports.
2.	Initial Data Exploration and Cleaning: Understanding the dataset and preprocessing.
3.	Targeted Data Exploration: Gaining deeper insights into employees who have resigned and visualizing key dependencies.
4.	Model Selection and Building: Choosing classification models, building them, and comparing their performance.
5.	Analysis of Modeling Results: Evaluating the model and interpreting the findings.

Dataset

The dataset consists of 15,000 rows and 10 columns, with each row representing an employee who is currently working or has worked at Salifort Motors.

The initial source of the dataset is available on Kaggle: HR Analytics and Job Prediction.

# Key takeaways. 

1. Project Load and Work Hours: Our analysis identified the number of projects and average working hours as the most significant factors influencing employee resignations.
 ![Unknown](https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/8ff374fc-431a-45e9-ab36-8c5b933d88f0)

 Interestingly, all employees who participated in more than six projects resigned. The following graph illustrates this trend  
 
 ![Unknown-2](https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/5cc15f65-2d8b-45f4-9713-95040f3cbbda)
 
 The turnover rate increases drustically if the employee works on more then 4 projects.

2. Potential Overwork Issue: The data suggests a potential issue with overwork within the analyzed company. The red line in the following graph represents the legal working time limit in France
  <img width="1034" alt="image" src="https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/7aa2ca18-2837-44c2-bd71-d1f9383876e5">

We can see that many employees appear to be exceeding this limit, potentially contributing to resignations.

3. The tenure variable is also an important predictor of employee resignation.
 <img width="1205" alt="image" src="https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/7c8a19f9-890a-47d0-b79a-41878378a539">

We can see that there are no employees who resigned after six years of experience at this company. We can also see that employees who resigned after two years of experience had good evaluation scores, indicating they were valuable to the company.

4. So we identified a group of employees who worked much more than average with high evaluation scores. We investigated this group of employees further, particularly examining the connection between their resignation and the fact of being promoted in recent years.

From this chart, we can draw two conclusions:

•	Very few individuals who were promoted in the last 5 years left the company.
•	Almost no individuals in the target group received a promotion.

We can assume that the lack of promotion could be one of the reasons for leaving the company.

<img width="1700" alt="image" src="https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/8ac59016-5cb1-4631-af59-bb51f288f9c2">


5. We created two linear regression models, one decision tree model, and one random forest model. We achieved a precision metric of 0.97 for the random forest model on the test data, indicating that we have a reliable model. We then analyzed the feature importance to understand the most important factors that increase the likelihood of an employee resigning.
 <img width="1254" alt="image" src="https://github.com/SergeiShadrin/coursera_salifort_capstone_project/assets/9164779/494f0726-aaf8-4557-a66e-cb3eb28d5d5c">
 
The results of the feature importance analysis in the construction of the random forest model differ slightly from the results of the decision tree model. Notably, this model assigns slightly less importance to the last evaluation. The first place is occupied by the satisfaction level, followed by the number of projects, the average hours worked, and tenure. The ‘satisfaction_level’ variable without further specification has low explanatory power. Consequently, we can conclude that in this company, the most important factors for employee departures were the excessive workload in terms of the number of hours worked and the number of projects employees were working on. Another important predictor is tenure: we observed that at the beginning of their careers, employees tend to leave their positions.
 
Recommendations Based on Analysis

The analysis of the models and the feature importance indicates that employees are overworked. Here are some recommendations to present to the stakeholders:

•	Cap the number of projects that employees can work on.
•	Consider promoting employees who have been with the company for at least four years or investigate further to understand their dissatisfaction.
•	Reward employees for working longer hours or do not require them to do so.
•	Inform employees about the company’s overtime pay policies if they are not familiar with them. Make workload and time-off expectations clear.
•	Hold company-wide and within-team discussions to address and understand the company work culture.
•	Do not reserve high evaluation scores for employees who work more than 200 hours per month. Implement a proportionate scale to reward employees who contribute more or put in more effort.

Instructions for Running the Notebook

1.	Prerequisites: Ensure you have Jupyter Notebook or Jupyter Lab installed along with the required Python libraries (e.g., pandas, numpy, matplotlib, seaborn, scikit-learn, etc.).
2.	Clone the Repository: Clone this repository to your local machine.
3.	Open the Notebook: Open the salifort_motors_project.ipynb file in Jupyter Notebook or Jupyter Lab.
4.	Run the Notebook: Execute the cells sequentially to replicate the analysis and the results.

Conclusion

This project provides insights into the factors influencing employee turnover at Salifort Motors and offers actionable recommendations to reduce the turnover rate. By building and evaluating predictive models, the analysis highlights the importance of workload and satisfaction in employee retention.

For more information, please refer to the notebook file.
