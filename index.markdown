# Fast Fourier Transform 알고리즘

202201626 이효민

### Fast Fourier Transform (FFT) 알고리즘
---
이산 푸리에 변환(Discrete Fourier Transform, DFT)과 그 역변환을 빠르게 수행해주는 알고리즘

#### DFT(Discrete Fourier Transform)
주파수×시간 축 데이터를 1:1로 변환하는 것

#### 시간복잡도

- DFT ->  O(n^2)
- FFT ->  O(nlogn)

#### 활용
- 오디오 및 음향 측정 과학 분야에서 중요한 측정 방법
- 디지털 신호처리에서부터 일기 예보나 기후 예측을 위해 편미분 방정식을 푸는 것까지 매우 많은 분야에서 활용

#### FFT 알고리즘 종류
- **Cooley – Tukey 알고리즘**
- Radix-2 FFT 알고리즘
- Radix-4 FFT 알고리즘
- 혼합 Radix FFT 알고리즘

### Cooley – Tukey 알고리즘
---
- 1965년 J. W. Cooley와 J. W. Tuckey가 발표한 가장 일반적으로 사용되는 FFT 알고리즘
- 보통 크기 N을 재귀적으로 2등분하여 길이가 2인 신호가 얻어질 때까지 분할 정복 알고리즘(Divide and conquer algorithm)을 적용하기 때문에 N = 2n인 경우에 많이 적용.
- 대용량의 자료 처리가 빠르게 가능하게 함.
- DFT를 작은 크기로 나누어서 다시 적용하기 때문에 다른 FFT 알고리즘의 기반이 됨.
