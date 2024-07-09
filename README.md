# coursera_salifort_capstone_project
This project is based on a fictional database proposed as part of the Google Advanced Data Analytics Professional Certificate program, which I completed on May 23, 2024.

Salifort Motors Employee Turnover Analysis

Overview

This project analyzes the employee turnover at Salifort Motors, an imaginary company. The goal is to understand the reasons behind the high turnover rate and to develop a predictive model to help prevent undesirable resignations. This project is based on a fictitious dataset provided as part of the “Google Advanced Data Analytics Professional Certificate” program.

Certificate

You can view the certificate for the completed program here.

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
 
 The the ternover rate increases drustically if the employee works on more then 4 projects.  

 	2. Potential Overwork Issue: The data suggests a potential issue with overwork within the analyzed company. The red line in the following graph represents the legal working time limit in France

We can see that many employees appear to be exceeding this limit, potentially contributing to resignations.

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
