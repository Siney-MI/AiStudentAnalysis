# AI Student Analysis: Impact on Academic Performance

[![Streamlit App](https://aistudentanalysis-crpctfpcyq3xtyatqugrkx.streamlit.app/)

https://aistudentanalysis-crpctfpcyq3xtyatqugrkx.streamlit.app/

## Overview
This project, developed by Sigourney Reipsch, explores the impact of Generative AI tools on the academic performance of college students. Built with **Python**, **Streamlit**, and **Scikit-Learn**, it provides an interactive web application that visualizes data trends and uses a K-Nearest Neighbors (KNN) Machine Learning model to predict whether a student's grades will improve based on their AI usage habits.

The analysis is based on the dataset *"AI Tools Usage by Indian College Students 2025"* from Kaggle.

## Key Features

### 1. Data Cleaning & Preparation
- Handles missing values and inconsistencies in the raw dataset (`Students.csv`).
- Standardizes categorical variables (e.g., standardizing capitalization for "Gemini", "ChatGPT").
- Extracts and expands multi-value columns (like `Use_Cases`) for granular analysis (saving to `use_case.csv`).
- Encodes categorical data into numerical formats suitable for Machine Learning.

### 2. Interactive Data Visualizations
The Streamlit app features a dedicated visualization dashboard where users can select different analytical views via a dropdown menu. Key insights visualized include:
- **Usage vs. Grades:** Analyzes if higher daily usage hours correlate with better grades (spoiler: it often plateaus or declines after ~2 hours).
- **Tool Preferences:** Shows the distribution of preferred AI tools (ChatGPT, Gemini, Copilot) among students.
- **Student Perception:** Visualizes how students self-assess the impact of AI on their grades vs. their trust in the tools.
- **Use Cases:** Breaks down the primary reasons students use AI (e.g., Coding Help, Assignments, Content Writing).
*Note: Each visualization includes an expandable textual analysis summarizing the key findings.*

### 3. Machine Learning Prediction (KNN)
- **Model Training:** Features a live interface to train a K-Nearest Neighbors classification model. It provides real-time accuracy metrics and a Confusion Matrix to evaluate performance (achieving ~66.11% accuracy).
- **Interactive Simulator:** Users can input hypothetical student profiles using sliders and dropdowns:
  - Daily Usage Hours
  - Field of Study (Stream)
  - Year of Study
  - Trust in AI
- **Live Prediction:** The app instantly predicts whether this specific profile will see an improvement in grades (1) or not (0), along with the calculated probability.


## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Siney-Ml/ai_student_analysis.git
   cd ai_student_analysis
   ```

2. **Install dependencies:**
   Ensure you have Python installed. Install the required libraries using pip:
   ```bash
   pip install streamlit pandas matplotlib seaborn scikit-learn
   ```

3. **Run the Streamlit app:**
   ```bash
   streamlit run app.py
   ```

## Author
* **Sigourney Reipsch** 
* Course: DataPy 25/26
