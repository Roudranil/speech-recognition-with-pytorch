# Audio Classification with CNN-LSTM networks

Data taken from [TensorFlow Speech Recognition Challenge](https:\\\\www.kaggle.com\\competitions\\tensorflow-speech-recognition-challenge\\overview).

| Model             | Num epochs | Validation acc | Test acc |
| ----------------- | ---------- | -------------- | -------- |
| Baseline          | 3          | 26.4           | 27.6     |
| CRNN              | 3          | 56.94          | 56.62    |
| Parallel CNN-LSTM | 6\*        | 84.92          | 84.29    |

Classification report for Parallel CNN-LSTM:

|              | precision | recall | f1-score | support |
| ------------ | --------- | ------ | -------- | ------- |
| zero         | 0.91      | 0.87   | 0.89     | 250     |
| one          | 0.71      | 0.9    | 0.79     | 248     |
| two          | 0.78      | 0.81   | 0.8      | 264     |
| three        | 0.81      | 0.91   | 0.86     | 267     |
| four         | 0.91      | 0.76   | 0.83     | 253     |
| five         | 0.86      | 0.73   | 0.79     | 271     |
| six          | 0.95      | 0.89   | 0.92     | 244     |
| seven        | 0.81      | 0.92   | 0.85     | 239     |
| eight        | 0.91      | 0.82   | 0.86     | 257     |
| nine         | 0.84      | 0.83   | 0.83     | 259     |
|              |           |        |          |         |
| accuracy     |           |        | 0.84     | 2552    |
| macro avg    | 0.85      | 0.84   | 0.84     | 2552    |
| weighted avg | 0.85      | 0.84   | 0.84     | 2552    |
