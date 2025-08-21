# Diabetes Risk Analysis
This is a predictive healthcare analytics project based on the [Pima Indians dataset](https://www.kaggle.com/datasets/nancyalaswad90/review/data) on Kaggle. This project aims to help patients and healthcare providers better understand an individual’s risk of developing Type 2 Diabetes by analyzing various health indicators and finding their predictive strenghts. Excel and Tableau are the main two tools that will be used in this analysis.

---

# 📊 About the Data

The data was found on Kaggle but was originally from the National Institute of Diabetes, Digestive and Kidney Diseases. All patients in the dataset are female, over 21 years of age, and of Pima Indian heritage. The dataset contains several medical predictor variables and one outcome variable which is whether the patient was diabetic or not. Dataset attributes included:

- Pregnancies: To express the number of pregnancies
- Glucose: To express the glucose level in blood
- BloodPressure: To express the blood pressure measurement
- SkinThickness: To express the thickness of the skin
- Insulin: To express the insulin level in blood
- BMI: To express the body mass index
- DiabetesPedigreeFunction: To express the diabetes percentage
- Age: To express the age
- Outcome: To express the final result 1 is YES o is NO



## 📁 Project Structure
- /README.md - What you are looking at right now! This provides a summary of the project and links to data, visualizations, and calculations
- /[data](https://github.com/jaylenroope-afk/DiabetesRiskPredictor/tree/main/data) - Contains raw and processed data, as well as summary statistics which was used in the calculation for diabetes risk
- /[Tableau](https://github.com/jaylenroope-afk/DiabetesRiskPredictor/tree/main/Tableau) - Includes png and twbx files containing important visualizations
- /[Presentation] - Slide deck used to present to stakeholders

---

## 🔧 Tools Used
- Excel (Data Cleaning, Sorting/Filtering, Pivot Tables, Summary Statistics)
- Tableau Public (Data Visualizations)
- Google Slides (Data Storytelling and Presentation)

---

# 🧐 Methods/Analysis
1. Pulled data from Pima Indians dataset on [Kaggle](https://www.kaggle.com/datasets/nancyalaswad90/review/data).
2. Cleaned the dataset on Excel. Started off by taking columns I did not need such as "DiabetesPedigree". Analyzed 7 columns such as BMI, Blood Pressure, Age, Insulin, Glucose, Skin Thickness, and # of Pregnancies. Then, got rid of impossible "zeros" that were in various columns (ex: BloodPressure cannot be "0" otherwise the patient would be dead).
3. To find which health indicators were better predictors on diabetic outcome, I first performed summary statistics on the 7 attributes I was analyzing. I used pivot tables to show the mean, min, and max, for both the diabetic and non-diabetic group and compared the difference.
4. To better understand the differences in summary statistics, I created a dashboard containing box-whisker plots for each of the 7 attributes. View the dashboard [here](https://public.tableau.com/app/profile/jaylen.roope/viz/ComparingHealthIndicatorsinDiabeticvsNon-DiabeticIndividuals/DemographicsandBodyMeasures).
5. Used the "CORREL" function to find the correlation of all 7 attributes with diabetic outcome.
6. Implemented a multivariate diabetes risk index by normalizing each individual's health attribute value as well as the correlation scores of the corresponding attribute. 
