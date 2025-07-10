# 🔍 Lock-in Thermography 기반 비파괴 결함 검사 시스템

## 📖 프로젝트 개요
MATLAB과 Lock-in Thermography 기법을 활용하여 전자 부품의 비파괴 결함 검사 시스템을 개발하였습니다. 주파수 잠금 기반의 적외선 이미징을 통해 미세한 결함도 정량적으로 검출 가능하도록 설계하고, SNR(신호대잡음비) 분석을 통해 성능을 개선했습니다.

## 🚀 기술 스택
- **언어:** MATLAB
- **기술:** Lock-in Thermography, Fast Fourier Transform (FFT), SNR 계산, 적외선 열화상 분석
- **하드웨어:** FLIR A655SC IR Camera, Keithley 2400 Source Meter

## 🛠 주요 기능
- 적외선 이미지 기반 결함 검출
- Time Periodic Signal 기반 FFT 분석
- 진폭 및 위상 이미지 생성 및 SNR 평가
- MATLAB App Designer 기반 통합 프로그램 개발
- 자동화된 데이터 시각화 및 CSV 저장

## 🖥 시스템 구성도
![image](https://github.com/user-attachments/assets/b4e1f762-81de-4a95-8403-86a4aa483dfe)

- IR 카메라 → 신호 동기화 → FFT 분석 → 결함 검출 → 결과 시각화

## 📊 결과 및 성과
- DBR 필름 유무에 따른 결함 검출 → SNR 최대 26.03dB까지 향상
- 신호 동기화 적용 시 기존 대비 5.5dB SNR 개선
- MATLAB App으로 실시간 데이터 취득 및 분석 자동화

## 📝 설치 및 실행 방법
```bash
# MATLAB 실행 후 프로젝트 폴더 내 app 또는 script 실행
# 필요한 경우 Image Acquisition Toolbox 설치
```

## 🔗 참고자료
- [시연 영상] https://youtu.be/D_BoAx4kQ_E
---
✅ 키워드: #MATLAB #LockinThermography #비파괴검사 #SNR분석 #FFT #IR이미지
