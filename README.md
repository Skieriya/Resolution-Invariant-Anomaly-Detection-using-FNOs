# Resolution-Invariant-Anomaly-Detection-using-FNOs

I recently came across FNOs ( Fourier neural operators ) during my personal research and by digging for sometime thier ability to learn the physics and predicting the state from that learned physics.
This led me into thinking of making FNOs learn the normal behavior with physics and predicting the anomalies with it ?? Cool right?

Anomalies here is generated with the following method:
1. Feed current data into the FNO.
2. FNO predicts what the data should look like next.
3. Wait for the actual next data point.
4. Calculate Residual = |Prediction - Actual|.

# If the system is normal, the FNO (with learned physics) predicts accurately → Low Residual.

# If there is an anomaly (e.g., a leak, a crack, a cyber-attack on sensors), the physics break 
  →
  The FNO predicts the "physics-compliant" outcome 
  →
  The actual data looks different  
  →
  High Residual (Anomaly Detected).

#Results
<img width="1456" height="998" alt="image" src="https://github.com/user-attachments/assets/5744b11b-ddbb-44ec-affb-6664d96b12d8" />


#Trained on 64x64 and tested on 128x128 ( where CNNs usually break )
<img width="1218" height="407" alt="image" src="https://github.com/user-attachments/assets/410e5c6f-3d5a-4314-a91f-d743a53bc4b1" />
