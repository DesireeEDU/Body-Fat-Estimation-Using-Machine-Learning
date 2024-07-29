# Body Fat Estimation Using Machine Learning Algorithms

## Project Overview

In this project, the goal is to develop a machine learning model to estimate body fat percentage based on anthropometric measurements. Body fat estimation plays a crucial role in health assessment and fitness evaluation, making it a significant application in health analytics.

## Project Phases

1. **Data Collection and Description:**
   - [Body Fat Prediction Data Set](https://www.kaggle.com/datasets/fedesoriano/body-fat-prediction-dataset)  (Kaggle)

      The dataset contains anthropometric measurements including weight, height, neck circumference, chest circumference, abdomen circumference, hip circumference, thigh circumference, knee circumference, ankle circumference, biceps circumference, forearm circumference, and wrist circumference. In addition, it           includes actual body fat percentage measured using reliable methods. All measurements are numeric. The data set includes 252 instance and does not have any missing values. The data source is a structured CSV file. 
     
      ![Circumference Measurements](https://github.com/DesireeEDU/44688-Data-Analytics-Capstone-Project-Desiree-Thompson/blob/main/circumference%20_measurements.png)

2. **Data Cleaning and Preparation:**
   
   - The dataset does not include any missing values and or outliers that would require further handling.
   
   - In preparation for for further analysis, three (3) additional features have been added:
      - BMI
      - BMI Body Fat
      - Navy Baody Fat

3. **Exploratory Data Analysis (EDA):**
   - Conduct EDA to understand the distribution of variables, relationships between features, and identify patterns in the data. Utilize visualizations and statistical summaries to gain insights.

4. **Machine Learning Modeling:**
   - Implement machine learning algorithms such as linear regression, decision trees, random forests, or support vector machines (SVMs) to build predictive models for estimating body fat percentage. Evaluate model performance using metrics like Mean Absolute Error (MAE) or Root Mean Squared Error (RMSE).

5. **Advanced Analysis (Module 5 Requirement):**
   - Showcase advanced skills by potentially exploring more sophisticated techniques such as ensemble methods, neural networks, or feature engineering to enhance model accuracy in predicting body fat percentage.

6. **Presentation of Results and Insights:**
   - Create a professional report using LaTeX detailing project objectives, data sources, cleaning methods, modeling approaches, and results. Include correctly-formatted code blocks to demonstrate technical proficiency.

7. **GitHub Repository:**
   - Maintain an active GitHub repository containing all code, data files, notebooks, and documentation related to the project. Ensure clear organization and documentation for reproducibility and review.

## Deliverables

**Overleaf/LaTex Report: [Body Fat Estimation Using ML Algorithms](https://www.overleaf.com/read/zbrdqhmnqgvt#574be8)**
   - Detailed report showcasing professional communication and technical skills.
     
**GitHub Repository: [44688 Data Analytics Capstone Project](https://github.com/DesireeEDU/44688-Data-Analytics-Capstone-Project-Desiree-Thompson)**
   - Well-structured GitHub repository with code, data files, notebooks, and documentation, including a clickable link in the report for easy access.

## Usage

**File Structure:**
- `.gitignore`: Specifies which files are to be ignored during a commit. 
- `requirements.txt`: File listing the dependencies required by the project.
- `data_analytics_capstone_notebook.ipynb`: Includes data cleaning, exploratory data analysis, and model implementation.
- `circumference_measurements.png`: Shows the features that relate to circumference measurements.
- `bodyfat.csv`: Original data set
- `updated_bodyfat.csv`: Modified data set

**Project Setup and Installation:**
1. Create a virtual environment
   ```
   python3 -m venv ds-venv
   ```

2. Activate the environment
     - On Windows:
      ```
      ds-venv\Scripts\Activate
      ```
     - On macOS and Linux
      ```
      source env/bin/activate
      ```
   
3. Install the 
   ```
   pip install -r requirements.txt
   ```

6. Run the Program:
   - Open the Jupyter Notebook
   ```
   jupyter lab
   ```
   - Navigate to 'data_analytics_capstone_notebook.ipynb' and run the cells to execute the analysis

## Implementation

**Feature Selection**

 Upon review of the features that were strongly correlated it was deterined that the following featues have the strongest correlation and potentially predictive ability. 
  - Abdomen
  - Biceps
  - Hip
  - Neck
  - Thigh

This is reflected in the correlation coefficients plot

   ![Correlation Coefficients](https://github.com/DesireeEDU/44688-Data-Analytics-Capstone-Project-Desiree-Thompson/blob/main/Correlation%20Matrix.png)

**Model Selction**

Employed multiple regression techniques that include:
 - Linear Regression
 - Polynomial Regression
 - Elastic Net

   ![Sample Linear Regression Code](https://github.com/DesireeEDU/44688-Data-Analytics-Capstone-Project-Desiree-Thompson/blob/main/Sample%20Linear%20Regression%20Code.png)

**Training and Testing**

The dataset was split into a training set that consist of 80% and a test set of
20%. Each model was trained on the same training and test dataset. 

**Results**

The results were summarized in the following table:

   ![Results Table](https://github.com/DesireeEDU/44688-Data-Analytics-Capstone-Project-Desiree-Thompson/blob/main/Results%20Table.png)

## 

**Author:**
Desiree Thompson

**Date Updated:**
July 28, 2024

**Acknowledgments:**
The project utilizes ChatGPT, an AI language model developed by OpenAI, for assistance in writing the README and providing guidance on software engineering practices.
