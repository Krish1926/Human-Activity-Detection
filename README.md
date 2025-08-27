# Human-Activity-Detection
\## \*\*🧐 Research Question\*\*

*\*What is the optimal combination of base learners and meta-learners to
achieve the best trade-off between accuracy and computational efficiency
in human activity detection?\**

\-\--

\## \*\*🎯 Aim\*\*

To **\*\*design, implement, and evaluate\*\*** an ensemble learning
framework combining various base learners and meta-learners to find the
optimal configuration for enhancing **\*\*human activity detection
accuracy\*\*** and **\*\*computational performance\*\***.

\-\--

\## \*\*📌 Objectives\*\*

\- 🔹 Perform an in-depth review of human activity detection research,
focusing on **\*\*ensemble learning models\*\***.  

\- 🔹 Prepare the dataset by **\*\*cleaning, normalizing\*\***, and
handling **\*\*imbalanced classes\*\***.  

\- 🔹 Develop and evaluate **\*\*base classifiers\*\***: Support Vector
Machine (SVM), k-Nearest Neighbors (k-NN), and Decision Tree (DT).  

\- 🔹 Train and evaluate **\*\*meta-learners\*\***: Logistic Regression
(LR), Gradient Boosting (GB), and Multi-layer Perceptron (MLP).  

\- 🔹 Construct and compare **\*\*stacking and voting ensembles\*\***,
evaluating them based on **\*\*accuracy, precision, recall,
F1-score\*\***, and **\*\*computational time\*\***.  

\- 🔹 Identify the **\*\*optimal ensemble configuration\*\*** for high
performance with efficiency.

\-\--

\## \*\*⚙️ Tools Required\*\*

\- **\*\*Python\*\***  

\- **\*\*Jupyter Notebook\*\*** / Any Python IDE  

\- **\*\*Scikit-learn\*\***

\-\--

\## \*\*🧰 Packages Used\*\*

\- \`numpy\`  

\- \`pandas\`  

\- \`scikit-learn\`  

\- \`imblearn\` (SMOTE oversampling)  

\- \`matplotlib\` / \`seaborn\` (data visualization)

\-\--

\## \*\*📝 Steps Included in the Research\*\*

1\. **\*\*Data Acquisition\*\***: HARSense dataset from NIT Meghalaya
via IEEE DataPort.  

2\. **\*\*Data Preprocessing\*\***: Handle null values, apply SMOTE for
class balancing.  

3\. **\*\*Base Classifiers Training\*\***: SVM, k-NN, Decision Tree with
5-fold stratified cross-validation.  

4\. **\*\*Meta-Learners Training\*\***: LR, GB, MLP on predictions from
base classifiers.  

5\. **\*\*Ensemble Models Construction\*\***: Stacking and voting
ensembles.  

6\. **\*\*Model Evaluation\*\***: Metrics---accuracy, precision, recall,
F1-score, training/testing time.  

7\. **\*\*Hyperparameter Optimization\*\***: GridSearchCV for
fine-tuning.  

8\. **\*\*Comparative Analysis\*\***: Identify best performing
combination.

\-\--

\## \*\*🗂 Total Number of Files\*\*

\- **\*\*file1:\*\*** \`All Users Combined.csv\` -- Contains the
combined sensor data of all subjects used for training and evaluating
the base classifiers (SVM, k-NN, DT).  

\- **\*\*file2:\*\***
\`Data_preprocessing_and_ML_implementation_of_Human_Activity_Detection.ipynb\`
-- Notebook for data cleaning, SMOTE oversampling, and implementation of
machine learning models.

 

\-\--

\## \*\*📊 Results\*\*

**\*\*Performance Metrics of Models:\*\***

\| Model Type \| Models \| Precision \| Recall \| F1-Score \| Accuracy
\|

\|\-\-\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\--\|

\| Base Classifiers \| SVM \| 0.75 \| 0.75 \| 0.74 \| 0.75 \|

\|                  \| KNN \| 0.89 \| 0.89 \| 0.89 \| 0.89 \|

\|                  \| DT  \| 0.80 \| 0.80 \| 0.80 \| 0.80 \|

\| Meta-learners    \| LR  \| 0.44 \| 0.45 \| 0.43 \| 0.45 \|

\|                  \| GB  \| 0.74 \| 0.74 \| 0.74 \| 0.74 \|

\|                  \| MLP \| 0.76 \| 0.76 \| 0.76 \| 0.76 \|

\| Stacking Ensemble \| Meta: LR  \| 0.90 \| 0.90 \| 0.90 \| 0.90 \|

\|                   \| Meta: GB  \| 0.86 \| 0.85 \| 0.85 \| 0.85 \|

\|                   \| Meta: MLP \| 0.90 \| 0.90 \| 0.90 \| 0.90 \|

**\*\*Training & Testing Times (seconds):\*\***

\| Model Type \| Models \| Training Time \| Testing Time \|

\|\-\-\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\-\-\-\-\-\-\--\|\-\-\-\-\-\-\-\-\-\-\-\-\--\|

\| Base Classifiers \| SVM \| 18.29 \| 5.20 \|

\|                  \| KNN \| 0.003 \| 2.16 \|

\|                  \| DT  \| 1.04  \| 0.012 \|

\| Meta-learners    \| LR  \| 0.32  \| 0.012 \|

\|                  \| GB  \| 13.17 \| 0.019 \|

\|                  \| MLP \| 20.82 \| 0.034 \|

\| Stacking Ensemble \| Meta: LR  \| 52.99 \| 7.17 \|

\|                   \| Meta: GB  \| 96.90 \| 8.88 \|

\|                   \| Meta: MLP \| 67.63 \| 8.17 \|

\-\--

\## \*\*💡 Conclusion\*\*

Stacking Ensemble with **\*\*LR\*\*** as meta-classifier is the most
effective configuration.  

\- Accuracy: **\*\*0.90\*\*** on all metrics  

\- Training time: **\*\*52.99s\*\***, Testing time: **\*\*7.18s\*\***  

\- Utilizes complementary strengths of **\*\*SVM, KNN, DT\*\***,
coordinated by **\*\*LR\*\*** as lightweight meta-learner  

\- Provides a **\*\*robust, scalable, practical solution\*\*** for
real-world wearable human activity detection

\-\--

\## \*\*🔜 Future Work\*\*

\- Explore **\*\*hierarchical ensembles\*\***  

\- Integrate **\*\*deep learning models\*\*** (CNNs, LSTMs) as base
learners  

\- Test on more **\*\*diverse datasets\*\***  

\- Deploy in **\*\*real-time wearable devices\*\*** to evaluate
practical applicability


