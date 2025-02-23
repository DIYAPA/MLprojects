# Math Score Prediction - End-to-End ML Project

## Overview
This project is an end-to-end Machine Learning (ML) system that predicts students' math scores based on various input features. The system is built with structured pipelines for:

- Data ingestion
- Data transformation
- Model training
- Model deployment using Flask

The trained model and transformer are saved as `.pkl` files and used for making predictions when a request is sent to the Flask API.

## Project Structure
```plaintext
├── __init__.py
├── __pycache__
├── artifacts
├── logger.py
├── pipeline
├── components
│   ├── __init__.py
│   ├── data_ingestion.py
│   ├── data_transformation.py
│   ├── model_trainer.py
│   ├── __pycache__
├── logs
├── templates
├── app.py
├── exception.py
├── notebook
├── utils.py
```

## Features
- Web interface using Flask
- Model predictions through a browser-based UI
- Pickle-based model storage and loading
- Pipeline-based approach for scalability and maintainability

## Installation

### 1. Clone the repository:
```sh
 git clone https://github.com/your-repo/ml-math-score-predictor.git
 cd ml-math-score-predictor
```

### 2. Create a virtual environment and activate it:
```sh
 python -m venv venv
 source venv/bin/activate  # On Windows use `venv\Scriptsctivate`
```

### 3. Install dependencies:
```sh
 pip install -r requirements.txt
```

## Running the Application

### 1. Train the model and save it:
```sh
 python components/model_trainer.py
```

### 2. Start the Flask server:
```sh
 python app.py
```

### 3. Open the browser and go to:
```
 http://127.0.0.1:1234/
```

## API Endpoints
- **Home Page:** `/`
- **Prediction Endpoint:** `/predictdata`

## Usage
- Users can input features such as gender, ethnicity, parental education, lunch type, test preparation course, reading score, and writing score.
- The application predicts the math score based on these inputs.

## Dependencies
- Python 3.x
- Flask
- Pandas
- NumPy
- Scikit-learn

## Future Enhancements
- Deploy the model on a cloud service
- Improve UI/UX for better user experience
- Add more features for better predictions

## License
This project is open-source under the MIT License.
