# Digital-Communication-Project
Project using Matlab and Simulink for 3rd year Computer Engineering course Digital Communication (ELC325). The project explores different modulation schemes such as BPSK, QPSK, FSK, QAM(16-64)

## BPSK Modulation
### Description
BPSK stands for Binary Phase Shift Keying. It's a modulation scheme where the face of the carrier signal is changed depending on the symbol sent. A symbol of value 1 has phase shift = 0, a symbol of value 0 has phase shift = 180.
### Instructions
Model parameters used:
1. Random Integer Generator
* Set size = 2
* Initial seed = 37
* Sample time = 1s
* Samples per frame = 100
2. AWGN Channel 
* Initial seed = 67
* Number of bits per symbol = 1
* Input signal power = 1
* Symbol period = 1s
### Scatter plots
![](BPSK/BPSK%20after%20noise.jpg)
![](BPSK/BPSK%20before%20noise.jpg)
### BER figure
![](BPSK/BPSK%20ber.jpg)
