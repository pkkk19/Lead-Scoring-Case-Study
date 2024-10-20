# X Education Lead Conversion Prediction

## Project Overview

X Education, an online course provider for industry professionals, faces a low lead conversion rate of approximately 30%. Despite generating numerous leads through various sources such as Google, direct traffic, and referrals, only a fraction of these leads convert into paying customers.

This project aims to improve the lead conversion rate by building a logistic regression model to identify "hot leads" — those most likely to convert. The model assigns a lead score to each potential customer, allowing X Education’s sales team to focus their efforts on the leads with the highest conversion probability. The target conversion rate set by the CEO is around 80%.

### Key Steps:

1. **Data Preprocessing**:
   - The dataset contains around 9000 leads with various attributes like Lead Source, Last Activity, and Total Time Spent on the Website.
   - Several irrelevant features were dropped (e.g., `Magazine`, `Prospect ID`, `Receive More Updates About Our Courses`) to streamline the analysis.
   
2. **Exploratory Data Analysis**:
   - Insights were gathered from various features:
     - **Lead Origin**: Approximately 52% of leads came from "Landing Page Submissions," with a 36% lead conversion rate.
     - **Current Occupation**: 90% of the leads were unemployed, but "Working Professionals" had a 92% conversion rate despite being only 7.6% of total leads.
     - **Lead Source**: Google had a lead conversion rate (LCR) of 40%, while references had the highest conversion rate at 91%.
     - **Last Activity**: "SMS Sent" had the highest conversion rate of 63%.
     - **Specialization**: Courses like Marketing Management and HR Management contributed significantly to conversions.

3. **Model Development**:
   - A logistic regression model was built to assign a lead score between 0 and 100 for each lead. The model uses features such as lead source, last activity, and current occupation to predict the likelihood of conversion.

4. **Evaluation**:
   - The model achieved:
     - **Train Data**:
       - Accuracy: 81.11%
       - Sensitivity: 80.74%
       - Specificity: 81.33%
     - **Test Data**:
       - Accuracy: 80.77%
       - Sensitivity: 80.27%
       - Specificity: 81.10%

### Goals of the Case Study

- Build a logistic regression model to assign a lead score between 0 and 100 to each of the leads.
- Identify the most promising leads for the sales team to focus on.
- Evaluate model performance using metrics like accuracy, sensitivity, and specificity.

## How to Use

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/x-education-lead-prediction.git
   cd x-education-lead-prediction ```
2. **Dependencies**:
  - Ensure that you have Python installed along with the necessary libraries. Install dependencies using:
    ```bash
    pip install -r requirements.txt```
3.**Run the Model**:
  - Execute the Jupyter Notebook to preprocess the data, build the model, and evaluate the results.

# Results

  - The logistic regression model successfully assigned lead scores to potential customers, with high   conversion probabilities identified.
  - The model’s sensitivity and accuracy were in line with the company’s goal of achieving a lead conversion rate of around 80%.

# Editing and Contributions
  - Reporting Issues: If you encounter any bugs or issues, please create an issue on GitHub under the Issues tab.
  - Contributing: Contributions are welcome! Feel free to submit pull requests to improve the model or add features.
  - Collaboration: For significant changes or new features, it's recommended to open a discussion to ensure smooth collaboration.
