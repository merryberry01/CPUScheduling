## CPU Schedulier Implementation
- 프로젝트에 사용된 커널은 debian linux kernel의 maintainer이신 한승훈 개발자의 저서 <64비트 멀티코어 OS 원리와 구조>에서 기술된 MINT64 OS를 사용했고, 리눅스 가상 머신(VMware, Ubuntu 22.04 LTS)에서 커널 빌드를 진행했다.
- 배포된 커널은 Multilevel Queue 기반의 Round Robin으로 동작한다. 따라서 이번 프로젝트에서는 책에서 기술되지 않은 SJF, FCFS 알고리즘을 직접 구현하고, 3가지 스케줄링 알고리즘(FCFS, RR, SJF)의 성능을 측정하여 비교, 분석한다.
