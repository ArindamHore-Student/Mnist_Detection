### **Handwritten Digit Classifier using Logistic Regression**

This project implements a handwritten digit classifier using **Logistic Regression** on the **MNIST dataset**. The classifier is trained to recognize digits (0-9) from 28x28 pixel grayscale images, achieving a classification model that can predict the correct digit from an input image.

#### **Key Features**:
- **Dataset**: The **MNIST dataset** is used, which contains 60,000 training images and 10,000 test images of handwritten digits.
- **Preprocessing**: The images are normalized to values between 0 and 1 for faster convergence and better performance.
- **Model**: A **Logistic Regression** model is employed for classification. The logistic regression is trained using the **One-vs-Rest (OvR)** strategy for multi-class classification.
- **Cross-Validation**: The model’s performance is evaluated using **3-fold cross-validation** to assess its generalization ability and to prevent overfitting.
- **Accuracy Evaluation**: The classifier is tested on a separate test set, providing an accuracy score as an indicator of its performance.

#### **Steps Involved**:
1. **Data Loading**: The MNIST dataset is fetched using the `fetch_openml` API.
2. **Preprocessing**: Pixel values are scaled between 0 and 1 to standardize the data.
3. **Model Training**: A Logistic Regression model is trained with the training data.
4. **Cross-Validation**: The model is validated using 3-fold cross-validation to check its consistency across different data splits.
5. **Testing**: The model is tested on a separate test set, and accuracy is calculated.

#### **Technologies Used**:
- **Python**
- **Scikit-learn**
- **NumPy**
- **OpenML** (for dataset loading)

#### **Results**:
The classifier’s performance is evaluated using accuracy metrics, and it achieves an accuracy score of approximately **99%** on the MNIST test set after training on the full dataset.
