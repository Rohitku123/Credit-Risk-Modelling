Credit Risk Modelling Project: PD, LGD, EAD
This repository contains a comprehensive end-to-end implementation of a Credit Risk Modelling framework, focusing on the development of the three key risk components used under Basel II/III Internal Ratings-Based (IRB) approaches:

Probability of Default (PD)

Loss Given Default (LGD)

Exposure at Default (EAD)



The models are developed using Python, based on real-world-inspired datasets (e.g., Lending Club) and follow a practical industry-standard methodology, useful for credit analysts, data scientists, and risk modelers.


 Project Objectives


Understand and model the credit risk of individual loans

Estimate the likelihood of default (PD), expected losses (LGD), and outstanding exposure (EAD)

Apply industry practices such as:

Weight of Evidence (WoE) & Information Value (IV)

Logistic and Linear Regression modeling



Feature binning & risk grouping

Model evaluation (AUC, Gini, KS, RMSE, R²)

Regulatory-compliant model structure




 Project Structure
Section	Description
Data Preprocessing	Handling missing values, outliers, variable transformations
PD Modeling	Fine & coarse classing, WoE encoding, logistic regression, evaluation
LGD Modeling	Regression on recovery rate, linear regression, log transformations
EAD Modeling	Usage given default modeling using linear regression
Model Validation	KS-statistic, AUC, ROC curves, residual analysis



Technologies Used
Python: Data preprocessing, modeling, and evaluation



Libraries: pandas, numpy, matplotlib, seaborn, sklearn, statsmodels



 Key Techniques
Weight of Evidence (WoE) Transformation: Converts categorical variables for PD modeling

Information Value (IV): Feature selection based on predictive power

Binning Techniques: Fine and coarse classing for continuous variables

Model Evaluation: ROC, AUC, KS, adjusted R², RMSE




 Insights Gained
PD model helps estimate the probability of default using borrower attributes.

LGD model provides insight into how much is lost if a default occurs.

EAD model helps predict the exposure amount at the point of default.

Combining these three gives the Expected Loss (EL):
EL = PD × LGD × EAD




 How to Use
Clone this repo:

bash
Copy
Edit
git clone https://github.com/yourusername/credit-risk-modeling.git
Install required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the Jupyter Notebook:

bash
Copy
Edit
jupyter notebook Credit\ Risk\ Modelling\ Project\ PD\ LGD\ EAD.ipynb
License
This project is open-source and available under the MIT License.

Acknowledgements
Inspired by industry practices and academic methodologies

Datasets inspired by platforms like Lending Club and public data repositories

