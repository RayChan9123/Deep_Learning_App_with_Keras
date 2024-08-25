# Tesla Stock Prediction with RNN

This project focuses on predicting Tesla's stock price using a Recurrent Neural Network (RNN) built with TensorFlow and Keras. Below is a summary of the key concepts and techniques I have learned throughout the project.

## Key Concepts Learned

### 1. Data Loading and Preprocessing
- **Pandas for Data Handling**: Loaded and manipulated datasets using pandas.
- **Feature and Target Extraction**: Extracted features and target variables from the dataset using `iloc`.
- **Train-Test Split**: Used `train_test_split` to split the dataset into training and testing sets.
- **Data Scaling**: Applied `MinMaxScaler` to scale features and target values, crucial for improving model performance.

### 2. Time Series Data Preparation
- **Data Reshaping for RNN**: Reshaped input data into the required 3D format `[samples, time steps, features]` for RNN models.

### 3. Recurrent Neural Networks (RNN)
- **Model Architecture**: Built an RNN model with three `SimpleRNN` layers to capture temporal dependencies:
  - First `SimpleRNN` layer with 256 units and `return_sequences=True`.
  - Second `SimpleRNN` layer with 128 units and `return_sequences=True`.
  - Third `SimpleRNN` layer with 64 units for final processing.
- **Dropout for Regularization**: Added `Dropout` layers with a rate of 0.25 after the first and second `SimpleRNN` layers to prevent overfitting.
- **Output Layer**: A final `Dense` layer with 1 unit for the prediction output.
- **Model Compilation**: Compiled the model using the Adam optimizer and Mean Squared Error (MSE) loss function.
- **Model Training**: Trained the model for 50 epochs with a batch size of 32 and a validation split of 0.1.

### 4. Model Evaluation and Visualization
- **Prediction and Inverse Transformation**: Predicted Tesla's stock prices on the test set and inverse-transformed the predictions.
- **Metrics Calculation**: Calculated the Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) to evaluate the model's performance.
- **Visualization**: 
  - Plotted actual vs. predicted values of Tesla's stock price.
  - Visualized training and validation loss over epochs.
- **Model Saving**: Saved the trained model for future use.

### 5. Performance Metrics
- **Error Metrics**: Explored metrics such as MAE, MSE, and R² for evaluating regression models.

## Project Structure
