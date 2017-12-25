# keras-malicious-url-detector

Malicious URL detector using char-level recurrent neural networks with Keras

The purpose of this project is to study malicious url detector that does not rely on any prior knowledge about urls

The training data is from this [link](https://github.com/vaseem-khan/URLcheck), can be found in "malicious_url_train/data/URL.txt"

# Deep Learning Models

The following deep learning models have been implemented and studied:

* LSTM: this approach uses LSTM recurrent networks for classifier with categorical cross entropy loss function
    * training: malicious_url_train/lstm_train.py (one-hot encoding)
    * predictor: malicious_url_predict/lstm_predict.py (one-hot encoding)
    * training: malicious_url_train/lstm_embed_train.py (word embedding)
    * predictor: malicious_url_predict/lstm_embed_predict.py (word embedding)
    
* CNN + LSTM: this approach uses CNN + LSTM recurrent networks for classifier with categorical cross entropy loss function
    * training: malicious_url_train/cnn_lstm_train.py 
    * predictor: malicious_url_predict/cnn_lstm_predict.py 