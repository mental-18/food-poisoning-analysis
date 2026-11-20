# 식중독 발생 현황 데이터 분석

## 1. 프로젝트 개요

2015년부터 2025년까지 국내 식중독 발생 통계를
활용하여 연도별, 월별, 계절별, 시설별
식중독 발생 현황과 특징을 분석한 프로젝트입니다.

## 2. 데이터 출처

- 제공 기관: 식품의약품안전처
- 제공 사이트: 식품안전나라
- 분석 기간: 2015~2025년
- 데이터 종류: 월별·원인시설별 식중독 발생건수 및 환자수
- 원본 파일 형식: Excel
- 정제 데이터 형식: CSV

[식품안전나라 식중독 통계](https://www.foodsafetykorea.go.kr/portal/healthyfoodlife/foodPoisoningStat.do?menu_no=519&menu_grp=MENU_GRP02)

## 3. 개발 환경 및 사용 라이브러리

### 개발 환경

- Python
- Jupyter Notebook
- VS Code
- Git / GitHub Desktop

### 사용 라이브러리 및 모듈

- pandas: 데이터 통합, 정제 및 분석
- openpyxl : Excel 파일 처리
- xlrd: .xls 형식의 Excel 파일 읽기

## 4. 프로젝트 구성 및 실행 방법

### 폴더 구성

- data/raw/: 수집한 원본 통계 파일

- data/processed/: 통합 및 정제된 데이터

- notebooks/: 데이터 정제, 검증 및 분석 코드

- results/: 분석 결과 Excel 파일

- README.md: 프로젝트 설명

### 실행 방법

1. Python 및 Jupyter Notebook 환경 준비

2. 프로젝트에 필요한 라이브러리 설치

3. notebooks 폴더의 data_inter.ipynb 파일 실행
    - data_cleaning.ipynb에 정의된 데이터 정제 함수 불러오기
    - 함수를 통해 데이터 정제 및 통합
    - 정제된 데이터를 csv로 저장

4. notebooks 폴더의 data_analysis.ipynb 를 실행
    - 정제된 csv 데이터 불러오기
    - 결측치, 중복값 데이터 검증

5. 분석 결과를 Excel 파일로 저장
    - data_analysis.ipynb 에서 분석 결과를 Excel 파일로 저장