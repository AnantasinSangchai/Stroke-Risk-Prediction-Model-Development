
# Stroke-Risk-Prediction-Model-Development
## Overview
โปรเจคนี้เป็นการพัฒนาแบบจำลองทำนายความเสี่ยงของโรคหลอดเลือดสมอง (Stroke) โดยใช้ Logistic Regression บนชุดข้อมูลจาก Kaggle (Shashwat Tiwari, 2021) ซึ่งมี 12 ฟีเจอร์ และ 43,400 รายการข้อมูล
## Workflow
1.  Exploratory Data Analysis (EDA) – วิเคราะห์และทำความสะอาดข้อมูล
2.  One-Hot Encoding – แปลงข้อมูลประเภท Categorical เป็น Numeric
3.  Model Training & Evaluation
    -   ใช้ Logistic Regression และ GridSearchCV
    -   เปรียบเทียบการ Resampling:
        -   Without Resampling
        -   OverSampling (SMOTE)
        -   UnderSampling
        -   Combining OverSampling & UnderSampling
4.  Model Evaluation
    -   Accuracy, F1-score, ROC-AUC
    -   Confusion Matrix & Classification Report
## Results
-   Accuracy: 99.12%
-   F1-score: 0.9911
-   AUC-ROC: 0.9985
-   False Positives: 5 ราย
-   False Negatives: 219 ราย (อาจพลาดการตรวจพบโรค)

ผลลัพธ์ชี้ให้เห็นว่าโมเดลสามารถแยกกลุ่มผู้ป่วยได้อย่างแม่นยำ แต่ยังต้องปรับปรุง Recall เพื่อลด False Negatives
## Author
นายอนันตสิน สังชัย
รหัสนักศึกษา 653450516-8
นักศึกษาสาขาวิทยาการข้อมูลและปัญญาประดิษฐ์ มหาวิทยาลัยขอนแก่น
