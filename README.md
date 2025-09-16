# Heart Stroke Prediction Web App

![Python](https://img.shields.io/badge/Python-3.9-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.25-orange.svg)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.3-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A user-friendly web application built with Streamlit to predict the likelihood of a heart stroke based on key health indicators. The prediction is powered by a trained Logistic Regression model.

## Demo

*[IMPORTANT: Add a screenshot or a short GIF of your running application here!]*

![App Screenshot](assets/screenshot.png) 

## Features

-   *Interactive Interface:* Users can input their health metrics using sliders and select boxes.
-   *Real-time Predictions:* Instantly get a prediction on stroke risk.
-   *Data-Driven:* Utilizes a machine learning model trained on health data.
-   *Easy to Use:* Simple and clean user interface for non-technical users.

## Technology Stack

-   *Backend & ML:* Python, Scikit-learn, Pandas, Joblib
-   *Frontend:* Streamlit
-   *Data Analysis:* Jupyter Notebook, Matplotlib, Seaborn

## Setup and Installation

Follow these steps to run the project on your local machine.

### Prerequisites

-   Python 3.8 or higher
-   Git for version control

### Installation Steps

1.  *Clone the repository:*
    bash
    git clone [https://github.com/](https://github.com/)[your-username]/[your-repo-name].git
    cd [your-repo-name]
    

2.  *Create and activate a virtual environment:*

    -   **Using conda (Recommended):**
        bash
        conda create --name stroke-env python=3.9
        conda activate stroke-env
        

    -   **Using venv:**
        bash
        python -m venv venv
        # On Windows
        .\venv\Scripts\activate
        # On macOS/Linux
        source venv/bin/activate
        

3.  *Install the required dependencies:*
    bash
    pip install -r requirements.txt
    

## How to Run the App

Once the dependencies are installed, you can run the Streamlit app with the following command:

```bash
streamlit run app.py
