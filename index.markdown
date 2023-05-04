# Fast Fourier Transform 알고리즘

202201626 이효민

### Fast Fourier Transform (FFT) 알고리즘
---
이산 푸리에 변환(Discrete Fourier Transform, DFT)과 그 역변환을 빠르게 수행해주는 알고리즘

#####시간복잡도

DFT ->  O(n^2)
FFT ->  O(nlogn)

#####활용

- 오디오 및 음향 측정 과학 분야에서 중요한 측정 방법
- 디지털 신호처리에서부터 일기 예보나 기후 예측을 위해 편미분 방정식을 푸는 것까지 매우 많은 분야에서 활용

### FFT 알고리즘 종류
- **Cooley – Tukey 알고리즘**
- Radix-2 FFT 알고리즘
- Radix-4 FFT 알고리즘
- 혼합 Radix FFT 알고리즘

#### Cooley – Tukey 알고리즘
---
1965년 J. W. Cooley와 J. W. Tuckey가 발표한 가장 일반적으로 사용되는 FFT 알고리즘이다.
