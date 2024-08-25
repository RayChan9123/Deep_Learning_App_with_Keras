# Tesla Stock Prediction with RNN

This project focuses on predicting Tesla's stock price using a Recurrent Neural Network (RNN) built with TensorFlow and Keras. Below is a summary of the key concepts and techniques I have learned throughout the project.

## Key Concepts Learned

### 1. Data Loading and Preprocessing
- **Pandas for Data Handling**: Learned how to load and manipulate datasets using pandas.
- **Feature and Target Extraction**: Extracted features and target variables from the dataset using `iloc`.
- **Train-Test Split**: Used `train_test_split` to split the dataset into training and testing sets.
- **Data Scaling**: Applied `MinMaxScaler` to scale features and target values, which is crucial for improving model performance.

### 2. Time Series Data Preparation
- **Data Reshaping for RNN**: Learned to reshape input data into the required 3D format `[samples, time steps, features]` for RNN models.

### 3. Recurrent Neural Networks (RNN)
- **Model Architecture**: Built an RNN model with three `SimpleRNN` layers to capture temporal dependencies.
  - First `SimpleRNN` layer with 256 units and `return_sequences=True`.
  - Second `SimpleRNN` layer with 128 units and `return_sequences=True`.
  - Third `SimpleRNN` layer with 64 units for final processing.
- **Dropout for Regularization**: Added `Dropout` layers with a rate of 0.25 after the first and second `SimpleRNN` layers to prevent overfitting.
- **Output Layer**: A final `Dense` layer with 1 unit for the prediction output.
- **Model Compilation**: Compiled the model using the Adam optimizer and Mean Squared Error (MSE) loss function.

### 4. Performance Metrics
- **Error Metrics**: Explored metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) for evaluating regression models.

### 5. Visualization
- **Matplotlib for Plotting**: Utilized `matplotlib` to visualize the results, including loss curves and predictions.

## Project Structure
