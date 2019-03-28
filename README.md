# DigitalCommunication
## To reproduce the figures
1-Make sure you have matlab with communication toolbox

2-type bertool in matlab command window

3-click on the Monte Carlo tab

4-set Eb/En range to -10:1:10

5-Browse the .slx file of the modulation scheme you want to simulate

6-type in the BER variable which will be the name of the modulation scheme

7-click plot



## 1-BPSK modulation scheme
BPSK is a two phase modulation scheme, where the 0’s and 1’s in a binary message are represented by two different phase states in the carrier signal: θ=0∘ for binary 1 and θ=180∘ for binary 0.

To modulate with BPSK using simulink i've used the **BPSK Modulator Baseband** this block accepts column vectors input signals,the **Random Number Generator** is the input to the modulator
the output of BPSK is then fed to **AWGN Channel** which is a white noise channel ,the output of this channel is fed to **BPSK Demodulator Baseband**
### Paramters
1. Random number generator:
  - Set size:2
  - Samples per frame:100
2. BPSK Modulator Baseband:
  - Phase:0
3. AWGN channel:
  - Eb/No:EbNo
4. BPSK demodulator baseband:
  - phase:0
  
  ### Schemtatic
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/BPSK.PNG)
  ### Scatter plots
  Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseBPSK.jpg)
  
  after Noise Scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseBPSK.jpg)
  
  ### BER performance
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/BPSK_Graph.jpg)
 
## 2-FSK modulation scheme
   FSK is the digital modulation technique in which the frequency of the carrier signal varies according to the digital signal changes. FSK is a scheme of frequency modulation.
   ## Paramters 
1. Random number generator:
  - Set size:8
  - Samples per frame:100
2. M-FSK Modulator Baseband:
  - M-ary number:8
3. AWGN channel:
  - Eb/No:EbNo
4. M-FSK demodulator baseband:
  - M-ary number:8
 ### Schemtatic
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/FSK.PNG)
  ### Scatter plots
  Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseFSK.jpg)
  
  after Noise Scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseFSK.jpg)
  ### BER performance
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/FSK_Graph.jpg)

## 3-QAM16 modulation scheme
QAM is a modulation scheme that can be used to transmit analog signals or digital bit of streams,in QAM there exists two carriers having same frequency but shifted in phase by 90 degree (that doubles the BW)one is called I-carrier and the other one is the Q-carrier By varying the number of allowed amplitude variations, you can represent as many states(symbols) of information as you want at the 16 QAM we have 4 amplitude variations  
### Paramters 
1. Random number generator:
  - Set size:16
  - Samples per frame:1000
2. Rectangular QAM Modulator Baseband:
  - M-ary number:16
3. AWGN channel:
  - Eb/No:EbNo
4. Rectangular QAM demodulatorr baseband:
  - M-ary number:16
 ### Schemtatic
  Schemtaic
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM16.PNG)
  ### Scatter plots
  Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQAM16.jpg)
  
  after Noise Scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQAM.jpg)
  
  ### BER performance
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM16_Graph.jpg)
  
## 4-QAM64 modulation scheme
QAM64 allows 8 amplitude variations 
### Paramters 
1. Random number generator:
  - Set size:64
  - Samples per frame:1000
2. Rectangular QAM Modulator Baseband:
  - M-ary number:64
3. AWGN channel:
  - Eb/No:EbNo
4. Rectangular QAM demodulatorr baseband:
  - M-ary number:64
 ### Schemtatic
  Schemtaic
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM64.PNG)
  
  ### Scatter plots
  Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQAM64.jpg)
  
  after Noise Scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQAM64.jpg)
  
  ### BER performance
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM64_Graph.jpg)
  
## 5-QPSK
Quadrature phase shift keying (QPSK) is a modulation technique, which  transmits two bits per symbol. QPSK modulates the data in 4 different phases and that leads to doubling the data rate  
### Paramters 
1. Random number generator:
  - Set size:4
  - Samples per frame:100
2. QPSK Modulator Baseband:
  - Phase offset:pi/4
3. AWGN channel:
  - Eb/No:EbNo
4. QPSK demodulatorr baseband:
  - Phase offset:pi/4
 ### Schemtatic
  Schemtaic
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QPSK.PNG)
  ### Scatter plots
  Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQPSK.jpg)
  
  after Noise Scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQPSK.jpg)
  
  ### BER performance
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QPSK_Graph.jpg)
