# Price Prediction Model  

## Overview  
This project is a machine learning pipeline for predicting prices based on input features. It utilizes MLflow for experiment tracking and includes a deployment script for serving predictions.  

## Features  
- **ML Pipeline**: Trains a model for price prediction.  
- **MLflow Integration**: Tracks experiments and model performance.  
- **REST API for Prediction**: Allows real-time predictions via HTTP requests.  

## Project Structure  
- `run_pipeline.py`: Runs the ML pipeline and logs experiments in MLflow.  
- `run_deployment.py`: Deploys the trained model as a web service.  
- `sample_predict.py`: Sends sample prediction requests to the deployed model.  
- `config.yaml`: Configuration file for model training.  
- `requirements.txt`: Dependencies for running the project.  

## Installation  
```sh  
pip install -r requirements.txt  
```

## Running the Pipeline  
```sh  
python run_pipeline.py  
```
After execution, start MLflow UI:  
```sh  
mlflow ui --backend-store-uri 'file:./mlruns'  
```

## Making Predictions  
Once the model is deployed, use `sample_predict.py` to test predictions:  
```sh  
python sample_predict.py  
```

## License  
This project is open-source and available for use under the appropriate license.  
