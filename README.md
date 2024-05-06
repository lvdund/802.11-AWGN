# 802.11-AWGN
- Bài tập lớn môn Mô hình hóa hệ thống và các phương pháp mô phỏng số-2-23 (BK01) với mã lớp ET6191-2-23 (BK01)
- Matlab R2018b

1. Steps involved for Transmitter:
  - Generate random input sequence and map the signals

  - Generate 64 samples with Nused=52,Nleft=6,Nright=5,Ndc=1
  
  - Converting this 64 point samples from Serial to Parallel and taking IFFT
  
  - Generate 16 cyclic prefix and append to 64 point making total 80 samples
  
  - Add AWGN to the Sample

2. Steps involved in Receiver structure
 
  - Removing 16 cyclic prefix Nleft,Nright and Ndc

  - Taking FFT of 64 point sample
  
  - Demodulate the signal and compare with the input transmitted signal and calculate the BER
  
