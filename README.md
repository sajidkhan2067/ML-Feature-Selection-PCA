# PCA (Principal Component Analysis)
PCA is a dimensionality reduction technique commonly used in machine learning and data analysis. While PCA is primarily used for dimensionality reduction, it can also be employed for feature selection, albeit indirectly. 
Steps:
1. Wireshark is used to create a .pcap file from network traffic. Then this [dataset](https://ieee-dataport.org/documents/dosddos-attack-dataset-5g-network-slicing) is created.
2. CICIFlowMeter converts 84 features from a .pcap file to a .csv file.
3. PCA calculates the top 10 features based on the variance shown in the table below. PCA was calculated using the’sklearn’ library of Python.

| Serial | Features            | Variance (%) |
|--------|---------------------|--------------|
| 1      | Protocol            | 18.446       |
| 2      | Flow Duration       | 14.115       |
| 3      | Tot Fwd Pkts        | 11.918       |
| 4      | Tot Bwd Pkts        | 9.539        |
| 5      | TotLen Fwd Pkts     | 4.649        |
| 6      | TotLen Bwd Pkts     | 3.627        |
| 7      | Fwd Pkt Len Max     | 3.564        |
| 8      | Fwd Pkt Len Min     | 3.350        |
| 9      | Fwd Pkt Len Mean    | 3.298        |
| 10     | Fwd Pkt Len Std     | 2.785        |
