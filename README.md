# Digital-Communication-Project
Project using Matlab and Simulink for 3rd year Computer Engineering course Digital Communication (ELC325). The project explores different modulation schemes such as BPSK, QPSK, FSK, QAM(16-64)

## 1.BPSK Modulation
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
Simulation time = 1000000
The reason for this is that BPSK has very low BER values, so unless the simulation time is long enough, the BER tends to -inf at high db values
### Scatter plots
![](BPSK/BPSK%20before%20noise.jpg) ![](BPSK/BPSK%20after%20noise.jpg)
### Ber figure
![](BPSK/BPSK(semilogY).jpg)

## 2.QPSK Modulation
### Description
QPSK stands for Quatrature Phase Shift Keying. 
### Instructions
Model parameters used:
1. Random Integer Generator
Set size = 4
All others parameters are the same as above
2. AWGN Channel 
Same as above
Simulation time = 100000
### Scatter plots
![](QPSK/before%20noise.jpg) ![](QPSK/20after%20noise.jpg)
### Ber figure
![](QPSK/QPSK(semilogY).jpg)

## 3.FSK Modulation
### Description
FSK stands for Frequency Shift Keying. 
### Instructions
Model parameters used:
1. Random Integer Generator
Set size = 8
All others parameters are the same as above
2. AWGN Channel 
Same as above
Simulation time = 10000
### Scatter plots
![](FSK/FSK%20before%20noise.jpg) ![](FSK/FSK%20after%20noise.jpg)
### Ber figure
![](FSK/FSK(semilogY).jpg)

## 4.QAM16 Modulation
### Description
QAM stands for Quadrature Amplitude Modulation. The basic idea is using 2 carriers, sin and cos, who are 90 phase apart.
QAM16 means our symbol carries value of 4 bits at once. Each symbol differs from another by changing the amplitude and phase. 
### Instructions
Model parameters used:
1. Random Integer Generator
Set size = 16
All others parameters are the same as above
2. AWGN Channel 
Same as above
3. Modulator and demodulation
Normalization method = Average power
Simulation time = 1000000
### Scatter plots
![](QAM16/QAM16%20before%20noise.jpg) ![](QAM16/QAM16%20after%20noise.jpg)
### Ber figure
![](QAM16/QAM16(semilogY).jpg)

## 5.QAM64 Modulation
### Description
Same as QAM16 but supports 8 bits transmission per symbol. Note that this makes QAM64 more error prone as symbols are close on our constellation diagram. 
### Instructions
Model parameters used:
1. Random Integer Generator
* Set size = 64
* Sampling time = 0.1s
All others parameters are the same as above
2. AWGN Channel 
Same as above
3. Modulator and demodulation
Normalization method = Average power
Simulation time = 100000
### Scatter plots
![](QAM64/before%20noise.jpg) ![](QAM64/after%20noise.jpg)
### Ber figure
![](QAM64/QAM64(semilogY).jpg)