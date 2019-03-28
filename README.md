# DigitalCommunication
## To reproduce the figures
1-Make sure you have matlab with communication toolbox

2-type bertool in matlab command window

3-click on the Monte Carlo tab

4-set Eb/En range to -10:1:10

5-Browse the .slx file of the modulation scheme you want to simulate

6-type in the BER variable which will be the name of the modulation scheme

7-click plot
## General Paramaters
1. Random number generator:
  - Source of initial seed :Auto
  - Initial Seed: 37
  - Sample time:1
2. Raised cosine transmit filter:
  - Rolloff factor:0.2
  - Filter span in Symbols:8
  - Output samples per symbol:8
  - Linear amplitude filter gain:1
  -Input processing:Columns as channels
  -Rate options: Enforce single-rate processing
3. Raised cosine receive filter:
  - Rolloff factor: 0.2
  - Filter span in symbols:8
  - Input samples per symbol:8
  - Decimation factor:8
  - Decimation offset:0
  - Linear amplitude filter gain:1
  -Input processing:Columns as channels
  - Rate options :Enforce single-rate processing


## 1-BPSK modulation scheme

BPSK is a two phase modulation scheme, where the 0’s and 1’s in a binary message are represented by two different phase states in the carrier signal: θ=0∘ for binary 1 and θ=180∘ for binary 0.


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
  
  #### without raised cosine 
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/BPSK.PNG?raw=true)
  
  #### with raised cosine
  ![BPSK WITHOUT RAISED COSINE](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/BPSK_Raised.PNG)
  
  ### Scatter plots
  #### Before Noise scatter plot without raised cosine 
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseBPSK.jpg)
  
   #### Before Noise scatter plot with raised cosine 
   
   ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/BPSK_beforeNoise_Raised.jpg)


  
  #### after Noise Scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseBPSK.jpg)
  
  #### after Noise Scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/BPSK_AfterNoise_Raisedjpg.jpg)
  
  
  ### BER performance
  
  #### without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/BPSK_Graph.jpg)
  
  #### with raised cosine
  
 ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/BPSK_Raised_Graph.jpg)

 
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
  #### without Raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/FSK.PNG)
  
  ### Scatter plots
  #### Before Noise scatter plot
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseFSK.jpg)
  
  #### after Noise Scatter plot
  
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
  #### Without Raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM16.PNG)
  
  #### With Raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QAM16_Raised.PNG)
  ### Scatter plots
  #### Before Noise scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQAM16.jpg)
  
  #### Before Noise scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/beforeNoise_QAM16_Raised.jpg)
  
  #### after Noise Scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQAM.jpg)
  
   #### after Noise Scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/afterNoise_QAM16_Raisedjpg.jpg)
  
  ### BER performance
  #### without raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM16_Graph.jpg)
  
  #### with raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QAM16_GRAPH_Raisedjpg.jpg)

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
  #### Without raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM64.PNG)
  #### with raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QAM64_Raised.PNG)
  
  ### Scatter plots
  #### Before Noise scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQAM64.jpg)
  #### Before Noise scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/beforeNoise_QAM64_Raised.jpg)
  
  #### after Noise Scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQAM64.jpg)
  
  #### after Noise Scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/afterNoise_QAM64_Reduced.jpg)
  
  ### BER performance
  #### With raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QAM64_Graph.jpg)
  #### without raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QAM64_Raised_Graph.jpg)
  
  
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
  #### Without raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QPSK.PNG)
  #### With raised cosine
 ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QPSK_Raised.PNG)

  ### Scatter plots
  #### Before Noise scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/beforeNoiseQPSK.jpg)
  #### Before Noise scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/beforeNoise_QPSK_Raised.jpg)
  
  #### after Noise Scatter plot without raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/afterNoiseQPSK.jpg)
  #### after Noise Scatter plot with raised cosine
  
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/afterNoise_QPSK_Raised.jpg)
  
  ### BER performance
  #### Without raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/QPSK_Graph.jpg)
  #### With raised cosine
  ![BPSK SCHEMTAIC](https://github.com/loaiali/DigitalCommunication/blob/master/plots/Raised%20cosine/QPSK_Raised_Graph.jpg)
  
