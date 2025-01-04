# Phishing-Datasets-Analysis

<h2> Overview</h2>
<p>This project applies statistical analysis and machine learning techniques to detect phishing websites using the Phishing Websites Dataset from the UCI Machine Learning Repository. The dataset contains several features, such as URL length, the presence of pop-up windows, and other attributes to classify websites as either phishing or legitimate. The goal of this analysis is to explore patterns in the data and evaluate the differences between phishing and legitimate websites using methods like hypothesis testing and decision tree classification.
</p>

<h2>Key Features</h2>
<ul>
  <li><strong>Phishing Website Classification:</strong> Build and visualize a decision tree classifier using Gini impurity as a criterion.</li>
  <li><strong>Performance Metrics: </strong>Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1-score. </li>
  <li><strong>Statistical Testing:</strong>Conduct hypothesis testing (two-sample t-test) on the feature "popupwindow" to assess its significance in distinguishing phishing from legitimate websites.
 </li>
</ul>

<h2> Technologies Used </h2>
<ul>
  <li>Python</li>
  <li>scikit-learn</li>
  <li>matplotlib</li>
  <li>seaborn</li>
  <li>pandas</li>
  <li>scipy</li>
</ul>

<h2> Dataset</h2>
<p><strong>Source:</strong> <a href="https://archive.ics.uci.edu/ml/datasets/phishing+websites" target="_blank">Phishing Websites Dataset - UCI Repository</a></p>
    <p><strong>Features:</strong> Includes attributes such as URL length, number of pop-up windows, and other features relevant to phishing detection.</p>
    <p><strong>Target:</strong> Class labels indicating whether a website is phishing (-1) or legitimate (1).</p>
 </p>

<h2>Steps and Code Walkthrough</h2>
<ol>
  <li>The dataset is fetched from the UCI Machine Learning Repository and split into training and testing sets. Features and target labels are separated for modeling.</li>
  
<img width="639" alt="step 1 ss" src="https://github.com/user-attachments/assets/585a432d-fe40-4d48-822e-687845498bf0"/>

  <li> Decision Tree Classifier is created using the Gini impurity criterion to distinguish phishing from legitimate websites. </li>
 
<img width="639" alt="tree" src="https://github.com/user-attachments/assets/2664a8ba-1041-4441-976f-c2a49245019c"/>

<li>A graphical representation of the decision tree is created to visualize the feature splits and the decision-making process.</li>

<img width="639" alt="tree code 2" src="https://github.com/user-attachments/assets/e8e20dcc-9321-4446-baa3-5e198ff66140" />

<img width="639" alt="tree image" src="https://github.com/user-attachments/assets/a23809f1-ea70-4eaf-a657-6cf5683e8e1f" />

<li>Confusion marix is generated, comparing the predicted labels against the true labels to evaluate the model's performance.</li>

<img width="639" alt="matrix code" src="https://github.com/user-attachments/assets/03f0059f-124f-43cb-ab25-3e3e4e44c178" />
<img width="639" alt="matrix graph" src="https://github.com/user-attachments/assets/e53211bc-7a87-4200-9858-cfbbef3f797b" />

<li>Evaluation/performance metrics are printed.</li>
<img width="639" alt="metrics code" src="https://github.com/user-attachments/assets/d4226246-9ed5-445c-bdc7-cafeb79dd94a" />
<img width="639" alt="metrics result" src="https://github.com/user-attachments/assets/07bc9d81-a545-424d-b937-cae80098df2c" />

<li>A two-sample t-test is performed to assess whether there is a significant difference in the feature 'popupwindow' between phishing and legitimate websites. </li>

<img width="639" alt="hypo code" src="https://github.com/user-attachments/assets/ef492a84-d5e7-403b-9dc4-f44dcd545920" />

<img width="639" alt="hyp output" src="https://github.com/user-attachments/assets/e87acbec-a866-45f5-b097-bdf6a6d872aa" />

<h2> Results and Findings</h2>
<ul><li><strong>Decision Tree:</strong> The decision tree was able to classify websites as phishing or legitimate based on their features with an accuracy of 96%.</li>
<li><strong>Confusion Matrix: </strong>strong>The model correctly identified most phishing and legitimate websites but made a few errors (false positives and false negatives).</li>
<li><strong>T-Test Results:</strong>strong> The T-test for the "popupwindow" feature showed no significant difference between phishing and legitimate websites (p-value > 0.05), suggesting that this feature may not be useful for distinguishing the two classes in this dataset.</li>
</ul>

<h2> Takeaways</h2>
<p>This project demonstrates how machine learning and statistical analysis can be applied to solve cybersecurity challenges such as phishing website detection. While the decision tree model performed well overall, further exploration of additional features and machine learning techniques could improve the model's accuracy.</p>


 
