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

# Results
<img width="986" height="339" alt="download" src="https://github.com/user-attachments/assets/42494a1e-911d-43db-a5a6-983359cbbd56" />


# Trained on 421x421 and tested on 842x842 
<img width="1061" height="989" alt="image" src="https://github.com/user-attachments/assets/f2392699-19b2-4a50-bf9a-db83d506f53f" />
