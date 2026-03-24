# Resolution-Invariant-Anomaly-Detection-using-FNOs

I recently came across FNOs ( Fourier neural operators ) during my personal research and by digging for sometime thier ability to learn the physics and predicting the state from that learned physics.
This led me into thinking of making FNOs learn the normal behavior with physics and predicting the anomalies with it ?? Cool right?

Anomalies here is generated with the following method:
1. Feed current data into the FNO.
2. FNO predicts what the data should look like next by learning physics.
3. If you input anomalous data in it the error function will find calculate Residual = |Prediction - Actual| or abnormal physics which can be seen in the error map



# Results
<img width="1089" height="528" alt="image" src="https://github.com/user-attachments/assets/315ba6eb-a6f5-4d19-846a-dd84176dfb37" />



# Trained on 421x421 and tested on 842x842 
<img width="1061" height="989" alt="image" src="https://github.com/user-attachments/assets/86daaa2d-e46c-4d7d-8270-9f9ce1e9268f" />

It can also predict with on high res data while being trained on less res data
