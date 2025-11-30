**AI Semester Project: Intelligent Career Guidance System:**

 **Student Details:**

**Name:** Hamzah Ahsan
**SAP ID:** 56187
**Course:** Artificial Intelligence
**Section:** SE 5-2
**Instructor:** M. Usman Karim

**Project Overview:**

The Intelligent Career Guidance System works like a simple AI assistant that asks questions and suggests the best career path for a student.
The project uses concepts learned in the AI course such as:

  **1. Expert systems**
  **2. Reasoning**
  **3. Machine learning**
  **4. Data preprocessing**
  **5. CNN based text classification**

Although CNNs are mostly used for images, in this project a **1D Convolutional Neural Network** is used to analyze student data and classify them into different career categories.

**Dataset Description:**

  **1. Total Rows:** 1000
  **2. Columns:** 22 (features + target)
  **3. Target Column:** Recommended_Career_Path

**Why Preprocessing Was Needed?**

Raw data can’t be used directly because a CNN requires clean, numeric, and scaled data.

  **Steps done:**
     1. Handling missing values
     2. Label Encoding categorical columns
     3. Scaling numerical features
     4. One-Hot Encoding the target
     5. Train-Test splitting
     6. Reshaping data for CNN input

**Model Architecture (1D CNN):**

   The CNN model includes:
      **1. Conv1D Layer** – extracts important patterns
      **2. MaxPooling1D** – reduces unnecessary information
      **3. Second Conv1D + MaxPooling1D**
      **4. Flatten Layer**
      **5. Dense Layer (64 units) + Dropout (0.3)**
      **6. Output Layer (Softmax)** for predicting career category

**Compilation:**

  **1. Loss:** Categorical Crossentropy
  **2. Optimizer:** Adam
  **3. Metric:** Accuracy

**Training Details:**

   **1. Epochs:** 120
  **2. Batch Size:** 32
  **3. Validation Split:** 0.20

**Model Evaluation**

**Classification Report:**

   Displays precision, recall, and F1-score for each class.

**Confusion Matrix:**

   Shows predicted vs actual career categories.

Most predictions fall on the diagonal, meaning the model identified correct categories more often.


**Final Accuracy Results:**

 **After 120 epochs:**

  **1. Training Accuracy:** 91.34%
  **2. Validation/Test Accuracy:** 21.25%

**Conclusion:**

Through this project, I learned how to:
    1. Clean and preprocess a dataset
    2. Convert categorical data into numerical form
    3. Build and train a 1D CNN model
    4. Use accuracy/loss graphs for evaluation
    5. Generate a Classification Report and Confusion Matrix
    6. Calculate final test accuracy
