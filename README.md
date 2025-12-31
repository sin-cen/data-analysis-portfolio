# Data Analysis Portfolio

서비스 로그 데이터를 기반으로  
구매 전환율, 매출, 사용자 행동 지표를 분석한 프로젝트 모음입니다.

SQL을 활용해 지표를 집계하고,  
Python(pandas, matplotlib, seaborn)을 사용해 데이터를 분석·시각화했습니다.  
실제 서비스 데이터 분석 업무에서 사용하는 분석 흐름을 연습하는 데 목적이 있습니다.

---

## Main Project  
### 기기별 구매 전환율 및 매출 분석

#### 문제 정의
사용자가 이용하는 기기(PC, Mobile)에 따라  
구매 전환율과 매출 성과에 차이가 있는지 확인하고,  
기기별로 다른 운영 또는 마케팅 전략이 필요한지 판단하고자 했습니다.

#### 데이터 개요
- 사용자 로그 데이터
- 주요 컬럼: device, purchased, price, qty, stay_time
- 매출은 price × qty로 계산

#### 분석 내용
- 기기별 방문자 수, 구매자 수, 구매 전환율 집계
- 기기별 총매출 및 평균 주문 금액 비교
- 체류 시간과 구매 여부의 관계 분석
- SQL로 집계한 결과를 Python으로 시각화하여 비교

#### 분석 결과
- 모바일은 구매 전환율은 상대적으로 높지만 평균 주문 금액이 낮아 총매출 기여가 크지 않음
- PC는 체류 시간이 길수록 구매 확률과 주문 금액이 함께 증가하는 경향이 나타남
- 기기별 사용자 행동 패턴에 차이가 존재함

#### 해석
- 모바일 사용자는 빠른 구매 성향이 강해 간단한 구매 유도 방식이 적합
- PC 사용자는 비교·탐색 시간이 길어 상세 정보 제공이 더 효과적일 수 있음

---

## Sub Projects

### SQL 기반 데이터 집계
- JOIN, GROUP BY, HAVING을 활용한 지표 산출
- 실무에서 자주 사용하는 집계 유형 연습

### Python 데이터 전처리 및 시각화
- pandas를 활용한 데이터 정제 및 파생 변수 생성
- matplotlib, seaborn을 이용한 시각화
- 분석 결과 해석 연습

---

## Skills
- Python: pandas, matplotlib, seaborn
- SQL: JOIN, GROUP BY, 집계 함수
- Data Analysis: 데이터 전처리, 지표 계산, 결과 해석
- Tools: Jupyter Notebook, GitHub

본 저장소는 Python과 SQL을 활용한 데이터 분석 포트폴리오입니다.
실제 서비스 로그 데이터를 가정하여 전처리 → DB 적재 → SQL 분석 → Python 시각화 → 인사이트 도출까지
데이터 분석 전 과정을 실습 및 정리했습니다.

Python: pandas, numpy, matplotlib, seaborn

SQL: MariaDB (JOIN, GROUP BY, HAVING, Subquery)

DB 연동: SQLAlchemy, pymysql

분석 환경: Jupyter Notebook

시각화/배포: Streamlit (대시보드 형태)

