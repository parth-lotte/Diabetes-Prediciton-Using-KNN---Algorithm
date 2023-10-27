
# Diabetes Prediction Using KNN Algorithm

Diabetes is a chronic metabolic disorder that affects millions of people worldwide. It occurs when the body either does not produce enough insulin, the hormone that regulates blood sugar, or cannot effectively use the insulin it does produce. This leads to high levels of glucose (sugar) in the blood, which can damage organs and tissues over time.  Numerous health issues, such as heart disease, stroke, renal disease, nerve damage, blindness, and amputations, can be brought on by diabetes. The management of diabetes and lowering the risk of severe consequences depend heavily on early diagnosis and treatment. 

Predictive modelling is one method for locating people who could be at risk of acquiring diabetes. A statistical method called predictive modelling analyses data to forecast upcoming occurrences or behaviors. Based on variables including age, family history, body mass index (BMI), and blood glucose levels, predictive modelling can be used to identify those who are at a high risk of getting diabetes. 







## Dataset

The dataset used for diabetes prediction typically includes medical and demographic data for individuals, such as age, gender, BMI, blood pressure, and blood glucose levels. The dataset may also include information about family history of diabetes and lifestyle factors such as physical activity and smoking status.

The dataset may be collected from various sources, including electronic health records, medical surveys, and clinical trials. It is important that the dataset is representative of the population being studied to ensure that the predictive model is accurate and reliable.

Dataset used consists of **2000 entries of 8 labels Glucose, Blood Pressure, Insulin, BMI, Age, Pregnancies, Skin Thickness, Outcome** and the dataset is used from Kaggle.
## Algorithm Analysis
KNN is a reasonably simple classification technique that identifies the class in which a sample belongs by measuring its similarity with other nearby points.It is based on Supervised Learning technique. K-NN algorithm assumes the similarity between the new case/data and available cases and put the new case into the category that is most similar to the available categories

**Euclidean distance:**

The first step in KNN is to compute the distance between a query point and all the other points in the dataset. The most common distance metric used in KNN is the Euclidean distance, which is calculated as:
           
                 d(x, y) = sqrt((x1 - y1)^2 + (x2 - y2)^2 + ... + (xn - yn)^2)

where x and y are two data points with n features (x1, x2, ..., xn) and (y1, y2, ..., yn), respectively.

**Finding the K nearest neighbors:**
 
After computing the distance between the query point and all the points in the dataset, the next step is to find the K nearest neighbors to the query point. This is done by sorting the distances in ascending order and selecting the K nearest points. 

**Classification:**

For classification problems, the most common approach is to use majority voting to predict the class label of the query point. That is, we count the number of neighbors belonging to each class and choose the class with the most votes as the predicted class. 

**Regression:**

For regression problems, the most common approach is to use the average of the K nearest neighbors' labels as the predicted label for the query point. That is,

            f(x) = (1/K) * sum(y_i) 
            
 where f(x) is the predicted label for the query point x, K is the number of nearest neighbors, and y_i is the label of the i-th nearest neighbor.

## Data Visualization

![alt text](https://github.com/parth-lotte/Diabetes-Prediciton-Using-KNN---Algorithm/blob/main/Histogram.png)