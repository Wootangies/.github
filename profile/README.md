<div align="center">

# 우땅이 ⚡

### 제조 공정 전력사용량 예측 및 피크전력 분석

생산·전력 데이터를 기반으로 미래 전력사용량을 예측하고,  
최대전력 피크가 발생하는 조건을 분석합니다.

</div>

---

## About Us

**우땅이**는 KAMP 데이터를 활용해  
제조 현장의 전력사용량을 예측하고 피크전력 발생 조건을 분석하는 프로젝트 팀입니다.

단순히 예측 정확도를 높이는 것에 그치지 않고,

**데이터 품질 검증 → 전처리 → 예측 모델링 → 오차 분석 → 피크 분석 → 운영 개선안 도출**

까지 연결하는 것을 목표로 합니다.

---

## Project

### 제조 공정 전력사용량 예측

제조기업은 설비 가동, 생산량 변화, 제품 전환, 교대시간 등  
여러 생산 조건에 따라 전력사용량이 크게 달라질 수 있습니다.

본 프로젝트에서는 생산 및 전력 데이터를 활용하여  
향후 지정 시간 구간의 전력사용량을 예측하고,

- 예측오차가 크게 발생하는 생산조건
- 최대전력 피크가 발생하는 주요 조건
- 피크전력 감소를 위한 생산 운영 방안

을 함께 분석합니다.

---

## Analysis Pipeline

```text
Raw Data
   │
   ▼
Data Quality Check
   │
   ▼
Time-series Reconstruction
   │
   ▼
Feature Engineering
   │
   ▼
Model Training & Validation
   │
   ▼
Power Consumption Prediction
   │
   ├───────────────┐
   ▼               ▼
Error Analysis   Peak Analysis
   │               │
   └───────┬───────┘
           ▼
Operational Strategy
```

---

## Key Tasks

### 01. Data Processing

- 원본 데이터 품질 검증
- 시간축 정합성 확인
- 15분 단위 데이터 재구성
- 결측치 및 이상 데이터 처리
- 예측용 Feature 생성

### 02. Prediction Model

- 여러 회귀 모델 학습 및 비교
- Validation 데이터 기반 성능 검증
- MAE / RMSE / R² 기반 모델 평가
- Peak 구간 예측 성능 추가 분석

### 03. Peak Analysis

- 최대전력 발생 구간 탐색
- 생산조건별 Peak 발생 패턴 분석
- Peak 미탐지 구간 분석
- 예측오차가 큰 생산조건 분석

### 04. Simulation & Strategy

- 생산일정 변경 시나리오 분석
- 설비 동시 가동 조건 분석
- 피크 발생 가능 조건 탐색
- 피크전력 저감을 위한 운영 방안 제안

---

## Model Evaluation

예측 모델은 전체적인 회귀 성능뿐 아니라  
**실제 전력 운영에서 중요한 Peak 구간을 얼마나 잘 탐지하는지** 함께 평가합니다.

주요 평가 지표는 다음과 같습니다.

`MAE` · `RMSE` · `R²` · `Recall` · `F1` · `Peak MAE` · `Peak Bias`

---

## Tech Stack

### Data & Modeling

`Python` `Pandas` `NumPy` `Scikit-learn` `LightGBM`

### Analysis

`Jupyter Notebook` `Matplotlib`

### Collaboration

`Git` `GitHub`

---

## Repository Structure

```text
.
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── src/
│   ├── preprocessing/
│   ├── features/
│   ├── models/
│   └── analysis/
│
├── outputs/
│   ├── metrics/
│   ├── predictions/
│   └── figures/
│
└── docs/
```

> 대용량 원본 데이터 및 CSV 파일은 Git 저장소에서 제외하고 관리합니다.

---

## Workflow

```text
main
 │
 ├── preprocessing
 │
 ├── modeling
 │
 ├── analysis
 │
 └── report
```

각 작업은 별도 브랜치에서 진행하며  
검증이 완료된 변경사항만 Pull Request를 통해 `main`에 병합합니다.

---

<div align="center">

### ⚡ 우땅이

**Manufacturing Power Demand Prediction & Peak Analysis**

</div>
