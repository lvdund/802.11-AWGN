# 802.11-AWGN
- Bài tập lớn môn Mô hình hóa hệ thống và các phương pháp mô phỏng số-2-23 (BK01) với mã lớp ET6191-2-23 (BK01)
- Matlab R2018b

1. Steps involved for Transmitter:
  1)Generate random input sequence and map the signals

  2)Generate 64 samples with Nused=52,Nleft=6,Nright=5,Ndc=1
  
  3)Converting this 64 point samples from Serial to Parallel and taking IFFT
  
  4)Generate 16 cyclic prefix and append to 64 point making total 80 samples
  
  5)Add AWGN to the Sample

2. Steps involved in Receiver structure
 
  1)Removing 16 cyclic prefix Nleft,Nright and Ndc

  2)Taking FFT of 64 point sample
  
  3)Demodulate the signal and compare with the input transmitted signal and calculate the BER
  
