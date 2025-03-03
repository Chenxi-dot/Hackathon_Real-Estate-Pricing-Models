## Hackathon: Real Estate Pricing Based on XGBoost and Artificial Neural Networks

This is a hackathon project finished by the author **independently**, which aims to construct models to price real estate assets, mainly in six big cities in China.

There are **three main folders** in this project:

- Mid-term_Models
- Model_Validation_Report_for_peers
- Final-term_Models

We will briefly introduce the main content of each folder.

---

#### Mid-term_Models

In this section, the codes are mainly used to **clean data** and to do **feature engineering** jobs. I have selected over 40 housing features(including interaction terms), such as the longitude and latitude of the community, location, transaction time, house orientation, building area, elevator ratio, heating fee, and property fee. Due to the strict requirements, in this part I only used linear models, including **OLS, Lasso, Ridge, ElasticNet.** I also tried **Principal Component Analysis(PCA)** to reduce dimensions.

#### Model_Validation_Report_for_peers

In this section, we have thoroughly studied other team's work. As the team leader, I have made the outline of the model validation report, which also makes a great job in presentation during the class.

#### Final-term_Models

There is no limit at all in the final-term model. I have innovatively added POI information into the previous models. It utilized **points of interest(POI)** data from the PKU Open Data Research Platform, which includes 136 features such as supermarkets, hotels, subways, buses, ATMs, and factories. For each point of interest, two sub-features were constructed: the nearest distance and the number of POIs within 3km, resulting in over 300 final model features.

Ultimately, the article adopted **XGBoost** and <u>a five-layer hidden layer</u> **ANN** for model training and used a combination of grid manual tuning and Optuna Bayesian tuning. The final results were **0.83646** and **0.77606**, respectively.

---

#### Q & A

If you want to reproduce the articles or the result, please feel free to contact kenric.xi@gmail.com or wang884314766@ruc.edu.cn to ask for databases.