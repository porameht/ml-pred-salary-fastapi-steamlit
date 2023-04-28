# ML-Pred-Salary-FastAPI-Streamlit

This project aims to predict salaries based on various factors using machine learning models, leveraging FastAPI for API development and Streamlit for interactive visualization.

## Table of Contents

1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Usage](#usage)
4. [API Endpoints](#api-endpoints)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction

This machine learning project utilizes a pre-trained model to predict an individual's salary based on factors such as experience, education, location, etc. The project is built using FastAPI for creating a RESTful API and Streamlit for an interactive user interface.

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:

git clone https://github.com/yourusername/ml-pred-salary-fastapi-steamlit.git

2. Change the working directory:

```
cd ml-pred-salary-fastapi-steamlit
```

3. Create a virtual environment:

```
python -m venv venv
```

4. Activate the virtual environment:

- Windows:
  ```
  .\venv\Scripts\activate
  ```
- Linux/MacOS:
  ```
  source venv/bin/activate
  ```

5. Install dependencies:

pip install -r requirements.txt


## Usage

1. Start the FastAPI server:

```
uvicorn main:app --reload
```

2. Open another terminal window and activate the virtual environment as described in the installation step.

3. Launch the Streamlit app:

```
streamlit run app.py
```

4. Visit the Streamlit app in your browser at `http://localhost:8501` and the FastAPI documentation at `http://localhost:8000/docs`.

## API Endpoints

- `/predict` (POST): Accepts input data in JSON format and returns the predicted salary.

Example request payload:

```json
{
 "experience": 5,
 "education": "Bachelor",
 "location": "San Francisco"
}

Example response:

```json
{
    "predicted_salary": 85000
}

Contributing
Contributions are welcome! Please read the CONTRIBUTING.md file for guidelines on how to contribute to this project.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
