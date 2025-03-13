# Predicting Compressive Strength with ML

In the construction industry, the compressive strength of concrete is one of the most important indicators of the quality of building materials. This property reflects the ability of concrete to withstand compressive forces applied to it. Knowing the precise compressive strength of concrete before construction plays a vital role in the design of structures. We aimed to explore and analyze the accurate prediction of concrete compressive strength using machine learning.
The primary goal is to model the nonlinear relationships between features and concrete compressive strength using machine learning algorithms to optimize design and reduce the need for physical testing. This approach, in addition to reducing costs and time, helps increase prediction accuracy and optimize material composition.
The dataset consists of various materials that influence the composition and compressive strength of concrete. Cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, and fine aggregate are all measured in kilograms per cubic meter (kg/m³) of the concrete mix and are used as input features in the model. The age of the concrete is measured in days (ranging from 1 to 365) and indicates the time elapsed since mixing and setting. The model’s output variable is the compressive strength of concrete, measured in megapascals (MPa), which indicates the concrete's ability to resist pressure. The goal of the model is to predict the compressive strength of concrete (MPa) based on the various inputs.
To predict the compressive strength of concrete, I used the ExtraTreesRegressor model. This model is a type of decision tree algorithm that operates based on a collection of random trees. Key features of this model include:
High speed: ExtraTreesRegressor uses trees where splits are chosen randomly, making it faster than Random Forest.
Nonlinear modeling: The model is capable of identifying nonlinear relationships between features and the target variable.
Resistance to overfitting: By averaging multiple trees, the model naturally avoids overfitting.


![1739867179066](https://github.com/user-attachments/assets/efc9be3a-7f67-4603-bec1-12cacb6c1f87)


The model performed with acceptable accuracy and provided meaningful results. To evaluate the model’s performance, I used the R² metric. This metric shows how well the model has been able to predict the real changes in the data. In simple terms, R² tells us how close the model's predictions are to reality.
If R² is close to 1, the model is performing well, and predictions are accurate.
If R² is close to 0, the model has not been able to make good predictions and is no better than the mean of the data.


![1739867178909](https://github.com/user-attachments/assets/d8811647-a6db-4566-82d8-1890b64046e5)


In this case, the ExtraTreesRegressor model achieved an R² value of 0.9432, indicating its good performance in predicting the compressive strength of concrete.


![1739867179249](https://github.com/user-attachments/assets/2467555d-381e-40a0-b907-7df61bdbadd8)
