# 🔍 Lock-in Thermography 기반 비파괴 결함 검사 시스템

## 📌 프로젝트 개요
MATLAB과 Lock-in Thermography 기법을 활용하여 전자 부품의 비파괴 결함 검사 시스템을 개발하였습니다. 주파수 잠금 기반의 적외선 이미징과 FFT 분석, SNR 계산을 통해 결함 유무를 정량적으로 판별하며, 자동화된 시각화와 데이터 저장까지 지원하는 통합 시스템입니다.

## 📽 데모 영상
🔗 https://youtu.be/D_BoAx4kQ_E

## ⚙️ 주요 기능 요약
| 기능 | 설명 |
|---|---|
| 🔍 결함 검출 | 적외선 이미지 기반 Lock-in Thermography로 결함 위치 및 상태 검출 |
| 📈 FFT 분석 | Time Periodic Solver 기반 FFT 분석으로 진폭 및 위상 이미지 생성 |
| 📊 SNR 평가 | 결함 영역과 비결함 영역의 신호대잡음비(SNR) 계산 및 비교 |
| 🖥 시각화 UI | MATLAB App Designer로 실시간 데이터 시각화 및 자동 CSV 저장 |

## 🔧 구현 개요
- IR 카메라와 Source Meter 장치 → MATLAB 제어 → 신호 동기화
- FFT 변환으로 결함 이미지 생성 → SNR 계산
- App Designer 기반 시각화, 자동 CSV 저장, 결과 이미지 생성
- Time Transient Solver 대신 Time Periodic Solver 사용으로 수렴성 향상

## 🚀 실행 방법
```bash
# MATLAB 실행 후 프로젝트 폴더 내 app 또는 script 실행
# 필요한 경우 Image Acquisition Toolbox 설치
```

## 📁 프로젝트 구조
```
Lockin_Inspection_Project/
├── lockin_main.m              # 메인 실행 스크립트
├── lockin_app.mlapp           # App Designer UI
├── data/                      # 실험 데이터 폴더
└── images/                    # 결과 이미지 저장 폴더
```

## ✉️ 알림 조건
- 결함 감지 시 → SNR 향상 결과 리포트 자동 출력
- 필름 유무 비교 → 자동 Normalize 및 그래프 출력

## 📝 개발자 메모
- Time Periodic Solver 적용으로 수렴 안정성 확보
- MATLAB App으로 실시간 분석 및 자동화
- 신호 동기화 → SNR 향상 → 결함 검출 성능 개선

✅ 향후 계획:
- 자동 결함 보고서 PDF 생성
- AI 기반 결함 패턴 자동 분류
- 실시간 클라우드 데이터 업로드 및 분석
