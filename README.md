# Weather-Forecasting-with-ML
Here is the contextual overview of the provided code:

1. **Data Loading and Exploration:**
   - The code begins by loading historical weather data for training from a CSV file (`DailyDelhiClimateTrain.csv`). The dataset includes features such as mean temperature, humidity, wind speed, and mean pressure.

2. **Data Preprocessing:**
   - The selected features are normalized using Min-Max scaling to ensure that all variables are on a similar scale, which is a common practice in neural network training.

3. **Neural Network Model Building:**
   - A feedforward neural network model is constructed using the Keras Sequential API. The model architecture includes an input layer, a hidden layer, and an output layer with the appropriate number of neurons for predicting mean temperature, humidity, wind speed, and mean pressure.

4. **Model Compilation:**
   - The model is compiled with the Adam optimizer and the Huber loss function. Huber loss is chosen for its robustness to outliers compared to Mean Squared Error.

5. **Training on Training Dataset:**
   - The model is trained on the entire training dataset. Training involves adjusting the model's weights to minimize the chosen loss function over 100 epochs, with batch sizes of 16.

6. **Test Dataset Loading and Preprocessing:**
   - The test dataset (`DailyDelhiClimateTest.csv`) is loaded, and similar preprocessing steps are applied, including feature selection and Min-Max scaling.

7. **Model Fine-tuning on Test Dataset:**
   - The model is fine-tuned on the test dataset for an additional 10 epochs to adapt to the characteristics of the test data.

8. **Future Date Prediction:**
   - Future dates are generated, and a DataFrame is created with placeholder values for prediction. The last known values from the test dataset are used for simplicity.

9. **Prediction for Future Dates:**
   - The model predicts the values for mean temperature, humidity, wind speed, and mean pressure for the next 6 or 7 dates.

10. **Display of Predicted Values:**
      ![image](https://github.com/vr-jayashree5443/Weather-Forecasting-with-ML/assets/128161257/38a9f404-13a5-4f50-a137-920500a21abc)

    - The predicted values for each variable are organized into a DataFrame and printed, providing insights into the forecasted weather conditions for the specified future dates.
