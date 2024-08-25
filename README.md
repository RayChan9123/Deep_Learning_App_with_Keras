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
- **Model Architecture**: Gained experience in building RNN models using the `Sequential` API in Keras.
- **Layers**: Learned how to use `SimpleRNN`, `Dense`, and `Dropout` layers to create robust models.
- **Training and Evaluation**: Understood the process of compiling, training, and evaluating the model's performance.

### 4. Performance Metrics
- **Error Metrics**: Explored metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) for evaluating regression models.

### 5. Visualization
- **Matplotlib for Plotting**: Utilized `matplotlib` to visualize the results, including loss curves and predictions.

## Project Structure