# Student Marks Prediction Using Machine Learning

## Aim
To predict a student’s expected exam marks based on the number of hours studied using Machine Learning.

## Methodology
- Type: Supervised Learning (Regression)
- Model: Polynomial Regression (Degree = 2)

Polynomial Regression is used because the relationship between study hours and marks is not perfectly linear. Marks increase rapidly at first and then gradually saturate near the maximum.

## Dataset
- Input Feature: Study Hours (0.25 to 14 hours)
- Output Label: Marks (0 to 100)
- Multiple entries are present for the same study hours to represent real-world variation in student performance.

## Working
1. The dataset is loaded from a CSV file using Pandas.
2. The input feature (Study Hours) is separated from the output (Marks).
3. Polynomial features of degree 2 are generated to capture non-linear patterns.
4. A regression model is trained using the transformed data.
5. The user enters the number of study hours.
6. The trained model predicts the expected marks.
7. The predicted marks are restricted between 0 and 100 to ensure realistic output.

## Tools Used
Python, Pandas, NumPy, Scikit-learn

## Conclusion
The Machine Learning model successfully predicts student marks using study hours and can help educators identify students who may require additional academic support before exams.
