# 📚 Student Performance Analytics & Dashboard

This project analyzes student performance data and provides an
interactive dashboard for visualization and GPA prediction. It combines
data preprocessing, exploratory data analysis, and machine learning in a
single solution.

------------------------------------------------------------------------

## 📂 Project Structure

  ---------------------------------------------------------------------------------
  File                             Description
  -------------------------------- ------------------------------------------------
  `student_performance_data.csv`   Dataset containing student performance metrics
                                   such as test scores, attendance, study hours,
                                   GPA, and major.

  `Project.ipynb`                  Jupyter Notebook used for data exploration,
                                   cleaning, visualization, and model development.
                                   Serves as a development/analysis environment.

  `student_dashboard.py`           Streamlit application that creates an
                                   interactive dashboard for visualizing student
                                   performance metrics and predicting GPA.
  ---------------------------------------------------------------------------------

------------------------------------------------------------------------

## ⚙️ Features

-   **Data Cleaning & Preprocessing**
    -   Handles missing values for math scores and attendance rates.\
    -   Calculates an `average_score` across math, science, and English
        scores.
-   **Exploratory Data Analysis (EDA)**
    -   GPA distribution by major.\
    -   Average score per major.\
    -   Study hours vs GPA scatter plot.\
    -   Attendance vs GPA scatter plot.\
    -   Correlation heatmap for all features.
-   **Machine Learning Model**
    -   Linear Regression model to predict GPA using:
        -   Math Score\
        -   Science Score\
        -   English Score\
        -   Attendance Rate\
        -   Study Hours per Week\
        -   Average Score
-   **Interactive Dashboard**
    -   Built with **Streamlit** and **Plotly**.\
    -   Real-time GPA prediction with sliders for input features.\
    -   Visualizations update dynamically.

------------------------------------------------------------------------

## 🚀 How to Run

### 1️⃣ Install Dependencies

``` bash
pip install pandas plotly scikit-learn streamlit
```

### 2️⃣ Run the Jupyter Notebook (optional)

``` bash
jupyter notebook Project.ipynb
```

This allows you to view and edit the data analysis steps.

### 3️⃣ Run the Dashboard

``` bash
streamlit run student_dashboard.py
```

Then open the provided local URL (usually `http://localhost:8501`) in
your browser.

------------------------------------------------------------------------

## 📝 Dataset Overview

The dataset (`student_performance_data.csv`) should include at least
these columns:

-   `math_score`\
-   `science_score`\
-   `english_score`\
-   `attendance_rate`\
-   `study_hours_per_week`\
-   `gpa`\
-   `major`

------------------------------------------------------------------------

## 🖥️ Dashboard Screenshots

-   **GPA Distribution**: Histogram with box plot by major.\
-   **Average Score by Major**: Bar chart.\
-   **Study Hours vs GPA**: Scatter plot showing relationship between
    study hours and GPA.\
-   **Attendance vs GPA**: Scatter plot showing relationship between
    attendance and GPA.\
-   **Correlation Heatmap**: Interactive heatmap of feature
    correlations.\
-   **Predict GPA**: Sliders to input scores and attendance to predict
    GPA instantly.

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Support for additional datasets or new features (e.g.,
    extracurricular activities).\
-   Model comparison (Random Forest, Gradient Boosting, etc.).\
-   Exportable student-level reports.
