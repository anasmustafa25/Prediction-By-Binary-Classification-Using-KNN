# -
A Machine Learning project using **𝐊-𝐍𝐞𝐚𝐫𝐞𝐬𝐭 𝐍𝐞𝐢𝐠𝐡𝐛𝐨𝐫𝐬 (𝐊𝐍𝐍)** to classify Red Wine quality with max **𝐀𝐔𝐂 𝐬𝐜𝐨𝐫𝐞**. It transforms multiclass data into an actionable "Premium vs. Standard" binary classification through **𝐒𝐭𝐚𝐧𝐝𝐚𝐫𝐝𝐒𝐜𝐚𝐥𝐞𝐫** and optimized hyperparameter tuning.

𝐖𝐢𝐧𝐞 𝐐𝐮𝐚𝐥𝐢𝐭𝐲 𝐏𝐫𝐞𝐝𝐢𝐜𝐭𝐢𝐨𝐧: 𝐁𝐢𝐧𝐚𝐫𝐲 𝐂𝐥𝐚𝐬𝐬𝐢𝐟𝐢𝐜𝐚𝐭𝐢𝐨𝐧 𝐰𝐢𝐭𝐡 𝐊𝐍𝐍
This project transitions from theoretical Machine Learning concepts to a real-world implementation using the Wine Quality (Red) dataset.
The goal is to predict whether a wine is "Premium" (high quality) or "Standard" based on its chemical properties using the K-Nearest Neighbors (KNN) algorithm.
𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐎𝐯𝐞𝐫𝐯𝐢𝐞𝐰
Predicting exact quality scores (3–8) can be inconsistent due to subjective labeling. This project redefines the problem into a Binary Classification task, identifying wines with a quality score of 7 or higher as "Premium" ($1$) and those below as "Standard" ($0$).

𝐆𝐫𝐚𝐩𝐡𝐢𝐜𝐚𝐥 𝐀𝐧𝐚𝐥𝐲𝐬𝐢𝐬 & 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧

Histogram

<img width="889" height="882" alt="Screenshot 2026-04-05 235319" src="https://github.com/user-attachments/assets/ca6dcf9c-0c94-493b-b968-e2d1ab87ff3a" />




Pairplot

<img width="1675" height="878" alt="Screenshot 2026-04-05 235535" src="https://github.com/user-attachments/assets/3345707f-53fc-4ff2-b576-47b523990d62" />



𝐊𝐞𝐲 𝐅𝐞𝐚𝐭𝐮𝐫𝐞𝐬 & 𝐖𝐨𝐫𝐤𝐟𝐥𝐨𝐰Data Cleaning:
Handled missing values/zeros in citric acid using mean imputation to maintain data integrity.

Feature Scaling: Applied 𝐒𝐭𝐚𝐧𝐝𝐚𝐫𝐝𝐒𝐜𝐚𝐥𝐞𝐫 to normalize features (Alcohol, Sulphates, Acidity, etc.), ensuring equal weight during distance-based calculations in KNN.Hyperparameter Tuning: Conducted a recursive loop for $K$ values (1–14) to identify the optimal neighbor count.

Binary Labeling: Converted multiclass labels into a binary format to improve model precision and utility.

𝐓𝐞𝐜𝐡𝐧𝐨𝐥𝐨𝐠𝐲 𝐒𝐭𝐚𝐜𝐤 Language: 
PythonLibraries: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, MlxtendEnvironment: Jupyter Notebook 𝐌𝐨𝐝𝐞𝐥 𝐏𝐞𝐫𝐟𝐨𝐫𝐦𝐚𝐧𝐜𝐞 After optimizing the model to 𝐊=𝟏𝟏, 
the following results were achieved:Accuracy: ~90%AUC Score: 𝟎.𝟖𝟕 (87% ability to distinguish between classes)Evaluation Metrics: Confusion Matrix, ROC Curve, and Classification Report (Precision/Recall).

ROC Curve
<img width="622" height="670" alt="Screenshot 2026-04-05 232817" src="https://github.com/user-attachments/assets/6c121ce9-34d4-4f30-a65e-93e45c82da6c" />

