# Project Title
Anomaly detection for clothing dye issues based on Clothing Quality data.

# Why I do this project?
The clothing dyeing market is currently experiencing rapid growth. However, 40–45% of dyeing processes in textiles result in anomaly quality. Additionally, the disposal of anomaly products generates more than 270 kilograms of carbon dioxide annually. Therefore, anomaly detection in clothing dyeing is vital to improve quality and reduce environmental impact. SO, we chose the topic of 'Anomaly detection for clothing dye issues based on Clothing Quality data'.


# Project Process

**Pipeline**
- Here is the overall pipeline.

![image](https://github.com/user-attachments/assets/d4a9ab13-fa64-48c7-88df-19eee722d665)

**Preprocessing**
- Remove unnecessary features through the data EDA process.
- Eliminate duplicate data using domain knowledge.
- Create derived variables such as 'Input Weight/Length' and 'Input Weight/Volume' to improve performance.
- we used data normalization 
- **Data Ratio**: We set the ratio of train, validation, and test sets to 7:1.5:1.5.
  - For deviate-based anomaly detection, the training process utilized only normal data.
  - The test dataset was prepared with a 5:5 ratio of normal and anomaly data.
- Integrate data as shown in the image below.

![image](https://github.com/user-attachments/assets/8bac9b3c-c4aa-4287-91dc-b8cc4c2d47d9)

**Modeling**
- We used LOF, Isolation Forest, KDE, and CBLOF methods for anomaly detection.
- To improve performance, we performed hyperparameter-tuning using grid search.

**XAI**
- Shap (XAI) was used for the interpretation of the results.


# Result
+ Modelling results showed that the LOF model and IsolationForest model performed best.

![image](https://github.com/user-attachments/assets/2fa54957-eb80-470a-bfbd-85823b519cc6)


# contribution
- Reduction in anomaly rates leads to savings in raw material costs.
- Early detection of anomaly improves product quality.
- Saving discarded textiles, dyes, and energy provides environmental benefits.

# Difficult Point
- It was difficult for the project to process duplicate data in three datasets because domain knowledge was required.
- It was difficult to generate derived features to enhance anomaly detection performance.