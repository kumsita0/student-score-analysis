# Student-score-analysis
The goal is to setup Python environment, write Python code, and understand the format that we need to follow to solve similar problems.  The Python code file shows code, and should also show the results. 

# Student Score Analysis

This project uses Python to analyze student math and science scores.

## Features
- Calculate average scores
- Identify the highest scoring students
- Demonstrates Python basics using Jupyter Notebook

## Tools Used
- Python
- Jupyter Notebook
- Anaconda
- GitHub

<img width="893" height="668" alt="image" src="https://github.com/user-attachments/assets/9afbf5b4-c57b-4e75-910a-d281ada121ad" />

#code- 
# Student Score Dataset

students = [
    {"name": "Alice", "math": 85, "science": 90},
    {"name": "Bob", "math": 78, "science": 82},
    {"name": "Charlie", "math": 92, "science": 88},
    {"name": "David", "math": 75, "science": 80},
    {"name": "Emma", "math": 88, "science": 92}
]

# Calculate Average Math Score
total_math = sum(student["math"] for student in students)
average_math = total_math / len(students)

# Calculate Average Science Score
total_science = sum(student["science"] for student in students)
average_science = total_science / len(students)

# Find Student with Highest Math Score
highest_math_student = max(students, key=lambda x: x["math"])

# Find Student with Highest Science Score
highest_science_student = max(students, key=lambda x: x["science"])

# Display Results
print("Average Math Score:", average_math)
print("Average Science Score:", average_science)

print("\nStudent with Highest Math Score:")
print(highest_math_student["name"], "-", highest_math_student["math"])

print("\nStudent with Highest Science Score:")
print(highest_science_student["name"], "-", highest_science_student["science"])
