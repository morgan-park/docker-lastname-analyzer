# Lastname Analyzer

This web application has been developed with a Flask backend, which incorporates a deep learning model predicting ethnicity based on a user's input--specifically, a last name. It also includes a React frontend. Docker was employed to orchestrate two distinct containers for the backend and frontend, respectively.
<br>
<br>
## Machine Learning Model Architecture
The deep neural network model is designed to predict ethnicity based on a last name. It begins with the input layer, where a last name is taken as input. The input undergoes a data masking process ('MASK' layer). The masked data is then forwarded to the LSTM (Long Short-Term Memory) layer, consisting of 256 nodes. After masking, it is flattened and enters the "Dense" layer, which includes two layers with ReLU activation functions featuring 128 and 64 "neurons," respectively. Finally, the output layer, built with a Softmax activation function, predicts ethnicity based on the user input (last name).

![Model Architecture](https://github.com/morgan-park/docker-lastname-analyzer/assets/94096127/27ae3cf7-a498-4644-bec8-6c51d2fe326e)

## Web App
I deployed this web app using Azure Web Services. Click this link to visit: [Lastname Analyzer](https://black-mushroom-0e59c6310.4.azurestaticapps.net/)
