# Temperature-Based Water Flow Control System

## Overview

This project involves building a temperature-based water flow control system using a Raspberry Pi. The system utilizes a temperature sensor to measure temperature, and based on the temperature readings, it controls a relay module to manage water flow. 

Additionally, the project includes a machine learning model to predict water flow based on temperature data. The model is trained using both logistic regression and a neural network, and it is deployed using TensorFlow Lite for efficient inference on edge devices.

## Components

1. **Temperature Sensor**: Measures the temperature and sends data to the Raspberry Pi.
2. **Raspberry Pi**: Processes temperature data and controls the relay module.
3. **Relay Module**: Controls the water flow system based on signals from the Raspberry Pi.

## Project Structure

1. **Data Collection**:
   - Simulates temperature data and water flow based on a threshold (24°C).
   - Saves the simulated data to a CSV file.

2. **Data Preprocessing**:
   - Loads and preprocesses the data for model training.

3. **Model Training**:
   - Logistic Regression and Neural Network models are trained to predict water flow based on temperature.

4. **Model Evaluation**:
   - Evaluates model performance using classification metrics.

5. **Model Deployment**:
   - Converts the neural network model to TensorFlow Lite format for efficient deployment.
   - Defines functions to predict water flow using the TensorFlow Lite model.

6. **Web Interface**:
   - A Streamlit app to interact with the model and visualize predictions.

7. **Email Alerts**:
   - Sends email alerts when the temperature falls below the threshold.

8. **Real-Time Prediction**:
   - Provides real-time predictions and visualizations based on user input.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/temperature-water-flow-control.git
   cd temperature-water-flow-control


Install dependencies:


pip install -r requirements.txt
Set up and run the Streamlit app:

streamlit run app.py
Authenticate ngrok (if needed for remote access):

ngrok authtoken YOUR_NGROK_AUTHTOKEN
ngrok http 8501
Files
data/simulated_temperature_water_flow_data_large.csv: Simulated temperature and water flow data.
model/temperature_model_large.pkl: Trained Logistic Regression model.
model/temperature_model_nn.h5: Trained Neural Network model.
model/temperature_model_nn.tflite: TensorFlow Lite model.
app.py: Streamlit app code for web interface.
email_alerts.py: Email alert functionality code.
detailed_water_flow_predictions.log: Log file for detailed predictions.
Usage
Run the Streamlit app to interact with the model and visualize predictions:


streamlit run app.py
Real-time Prediction: Use the command-line interface to input temperature values and get predictions.

Email Alerts: Configure the email settings in email_alerts.py to receive alerts based on temperature thresholds.

License
This project is licensed under the MIT License. See the LICENSE file for details.


sql
Feel free to adjust any sections according to your specific requirements or additional features.





