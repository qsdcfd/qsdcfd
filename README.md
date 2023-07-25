
# Hie

[Notion Resume](https://bedecked-erigeron-eaa.notion.site/Analyst-Engineer-b50150d8695549398689925098f8f392?pvs=4)
[![Linkledin](https://img.shields.io/badge/Linkledin-blue?style=flat&logoColor=white)](https://www.linkedin.com/in/%EC%84%B8%ED%98%84-%EC%9D%B4-b35aa8241/)
[![Gmail Badge](https://img.shields.io/badge/-leesehyun01@gmail.com-c14438?style=flat&logo=Gmail&logoColor=white&link=mailto:devcseo@gmail.com)](mailto:leesehyun01@gmail.com) 


## 💬 About me

# 🪄Founded Experience.

## 두디스

유튜버들의 고민을 해결해주는 빅데이터 기반의 컨설팅 회사

**총 업무 기간: 진행 중**

*Data Scienctist*

2022.11~ing

- **Business Intelligence**

- **사내 데이터 분석 및 검색 엔진을 위한** **Data Pipeline 구축 by AWS**
   - OLAP
- **메신저, 모니터링 서버 QA 대응, 배포 및 운영 및 기획**
- **자연어 생성 모델 서비스 개발 및 기획**

- **Data 판매 전략**
---

# Work Experience.

## 윙크스톤파트너스

중소상공인 대상 데이터 기반 금융서비스 윙크스톤파트너스

**총 업무 기간: 진행 중**

Data Scienctist

2023.05 ~ ing

- **Business Intelligence**
    
    회사의 니즈:
    
    회사의 상황:
    
    Before / After
    
    - **워크로드와 비즈니스를 고려한 데이터 모델링 및 데이터 마트 설계**
        - 데이터 파이프라인 구축을 위한 Data Flow 도식화 후 전사에 교육 진행
        - *사용자 요구사항 정의서 기반으로 클라우드 기능 선정 및 데이터베이스 설계*
            - 당사/ 외주사의 데이터베이스를 정의(물리적 스키마)
                - 당사 DB: Maria DB, 외주사 DB: Postgre
                - Cloud: Mysql & MongoDB
            - 여러 데이터베이스와 테이블의 관계도(E-R모델) 설정[논리적스키마]
            - View 스키마 구성을 바탕으로 데이터 마트 생성
                - BI를 위한 데이터 시각화 도구 선정(Tableau, Kibana)
    - **사용자 요구 정의서 바탕으로 데이터 수집 및 스케쥴링**
        - 목적1 : 전사가 동일한 데이터를 보며 일할 수 있도록 기본적인 데이터 인프라 세팅 및 대시보드 제작
        - Airflow를 활용
            - 데이터 크롤링 주기 설정(1hour)
            - 크롤링 이슈 → slack 연동
            - 크롤링 데이터→ Object Storage →  Maria DB 적재
        - Django API 스케쥴러를 기반으로 로그 데이터 배치 및 실시간 데이터 수집을 통해서 정합성 이상 감지(외주사와 협업 진행)
            - Airflow는 log history는 남지만 저장되지 않는 이슈가 있다.
        - Hadoop Ecosystem기반 데이터 운영 효율화 및 자동화 파이프라인 구축
            - Spark 및 Hive 활용
        
    - **MLops 기획**
        - 현금 흐름 예측 / 상권분석을 위한 ML 모델 결과를 Docker-Kubernetes기반으로 저장
        - Product & Service적용을 위한 백엔드팀과 협업을 통해서 Restful API 배포 진행

## 이음메디컬세일즈플랫폼

3500여개 병원과 함께하는 CSO 업계1등 이음메디컬세일즈플랫폼

**총 업무 기간: 7개월**

Data Scienctist

2022.10-2023.04

- **Business Intelligence**
    
    회사의 니즈:
    
    회사의 상황:
    
    Before / After
    
    - **검색/조회 시스템 변경 및 추천시스템 개발**
        - VOC1 : 검색/조회 기능 강화
            - 제품 이름과 성분이 잘못된 약품 수정 진행
            - 성분별 의약품 Grouping by K-means Clustering
            - Query형 조회로 인해서 검색 속도가 느려짐
                - EC2 → Kinesis Streams→ Opensearch구조로 웹 크롤링 방식 진행
                - 검색 속도 20% 상승 및 속도 저하 문의 65% 감소
        - VOC2: 협업 필터링
            - 구매 데이터 기반인 협업 필터링 방식 진행
            - 공공데이터 API와 당사 데이터를 활용해서 LBS 시스템을 이용하여 의원별 추천시스템 진행
            - 폐쇄몰이라서 데이터가 작으므로 인기 제품 sorting방식
            - 동일 약품 대비 당사 매출에 이득이 되는 약품 추천을 위한 가중치 모델 구현
        - Gitlab& Jenkins를 활용하여 애플리케이션 프로그래밍 인터페이스 개발 및 테스트 자동화 수행
    - **추천시스템과 자연어처리를 활용하기 위한 당사 웹사이트 유저 분석 및 기술 기획 (**2022.10-2023.02)
        - 마케팅부터 최종 결제까지의 퍼널 전체 데이터를 보며 랜딩 페이지 기획/개발, 기존 홈페이지 대비 결제 전환율 150% 개선
        - 페르소나 구축
            - 폐쇄몰이라는 특성과 과거의 데이터를 활용하여 유저 세그먼트 진행
                - 한정된 지역, 한정된 병과라는 것을 통해서 사용자의 특징 파악하는 방식인 Attitudinal Segmentation 진행
        - 유저가 원하는 서비스를 Sentimental Segmentation 조사 진행
            - 수집된 VOC 데이터를 바탕으로 “추천시스템” 베타 버전 방식 수립
                - voc1: 제품과 성분 이름 명 조회가 느리다.
                - voc2: 유사한 약 정보 / 병과 정보를 바탕으로 추천 제품이 나오기
                - voc3: 전월 구매 데이터가 당월 장바구니에 담기도록
        - 당사 쇼핑몰 웹 사이트 내 유저 행동 파악
            - 유저의 Log 데이터를 Membership analysis방식으로 진행
                - GA활용
            - 디자이너와 함께 광고 CTR을 높이기 위해서 리치 미디어 광고와 검색 광고의 배치
        - 신규 유저(영업 담당자)가 구매까지 도달할 수 있도록 AARRR & Funnel을 Mix하여 진행
            - 폐쇄몰과 제약업계 특성상 한 번 유입된 유저는 크게 벗어나지 않기에 신규 유저 흡수가 중요
            - 단순 웹사이트 광고뿐만 아니라 신규 유저의 업력과 과거 이력 기반 관리형 포토폴리오 작성 및 정기적으로 배부
        - AWS RDS, Athena, Python, Spark sql(Pyspark), GA, DA
    - **자사의 수익성을 높이는 동시에 의사결정의 위험을 완화 목적인 Predictive Analytics Reporting(**2022.10-2023.01)
        - 기존의 KPI를 바탕으로 Risk 관리를 위한 새로운 KPI지표 설정
            - 기존 KPI로 잡지 못했던 매출 손해 및 증대 약품/회사 선별
            - 추가적인 수수료 조정을 통해서 자사 매출 10% 상승
        - 월 매출 담당자/물품 예상 매출 평가 모형 모니터링 개발
            - 영업 담당자의 매출/영업 관련 데이터 및 지역 유동인구,약국-병원등의 공공데이터를 활용해서 예상 담당자별 월 매출 및 전략적인 판매 약품 선정(Predict LTV, Power BI 활용)
            - 영업 담당자의 매출 18%증대, 회사 매출 5% 증가
                - 자사 매출의 격차 이유: 당사에게 이득이 되는 약품이 아닌 담당자에게 이득이 되는 약품 판매
                    - 과거 데이터 기반으로 Anomlay Detection기법을 통해서 **체리피커 담당자 checking.**
        - 업무 자동화(AWS, ML, Python, Fast API)
            - 사내 웹 사이트 개발 with 프리랜서 외주 업체
            - 평가 모형 및 Portofolio의 자동화
            - ML pipeline: S3→Sagemaker 이용
            - Data Pipeline: RDS → S3 → Athena → Quicksight
        - Sentimental Segmentation기법을 통해서 HR팀과 바뀐 방식에 대한 반응 파악을 위한 후속 모니터링 진행 문제를 해결하는 문화 확산

---

## **NIA**

공공데이터 기업매칭 청년인턴십은 공공데이터 분야 청년 인턴십을 통해 취업을 준비하는 청년들에게 일경험을 제공하고 전문 교육을 통해 역량 강화를 지원하기 위한 프로그램

**총 업무 기간: 4개월**

**Data Analyst**

**Apprentice**

2021.09-2021.12

- 데이터 품질 판별을 위한 KPI 지표를 기획/마케팅팀과 재설정한 후 전사에 교육 작업 진행
- 데이터 바우처 참여 기업이 제공한 정형 데이터(SQL)과 비정형 데이터(Python)을 활용하여 데이터 품질에 관한 보고서 및 대시보드 제작

---

# Lecture Experience.

**cobslab**

**AI & Data instructor**

2022.08 ~ ing

**총 업무 기간: 진행 중**

- **심사위원**
    - 모두의연구소 아이펠 파이널 프로젝트 심사위원
    - 모두의 와이디어랩 프로젝트 심사위원
- **강사**
    - 한국폴리텍대학교, 교수 및 임직원 대상 컴퓨터비전(Opencv, Pillow) 강의
    - 전주 문화 산업진흥원, 자연어처리 전문가 과정
    - 이스턴마스텍, 컴퓨터 비전 딥러닝 프로젝트
    - KETI 나노 데이터 , 머신러닝 프로젝트
- **코치**
    - 2023 LG전자, SW/ 딥러닝 전문가 과정
    - 2022 교원 대상 디지털 전환을 위한 AI전문가 과정 실습코치
- **멘토**
    - 성균관대학교, 대학생 대상 AI 기술 멘토
    - 스마트인재개발원, k digital training Final Project 멘토(2022.11 ~)
    - 지역ICT 이노베이션 확산사업 전문가 멘토링 프로그램 개발/직무 멘토

---

## Freelancer

**Data Scientist**

2023.01-2023.03

**Data Scientist**

2023.02-2023.02

### Naver ENTRY

- 엔트리를 이용하는 학생들의 학년별 선호/비선호 프로젝트의 공통점/차이점 분석 보고서 프로젝트
    - 10GB, 1억만 건의 데이터를 Google Bigquery, AWS S3, Python을 활용하여 데이터 분석 후 Power BI로 시각화 진행
    - 초등학생 저학년 ~ 고등학생까지 이용자의 선호/비선호 프로젝트를 조회수, 좋아요, 북마크를 통해서 분류
    - 선호/비선호 프로젝트를 형태소 분석(KoNLPy, Keybert)를 활용한 후 TF-IDF를 통해서 그룹화
    - LDA를 활용하여 프로젝트의 주제 선정을 편의성을 위한 Topic Modeling 진행
    - 분석 보고서를 바탕으로 소비자의 니즈 파악하여 유저의 집중 시간 평균 대비 15% 상승 및 좋아요 수 10% 증가

### 소상공인 카페 매장 데이터

*소상공인의 카페 이용객 정보 데이터 데이터 분석을 통한 리워드 보상 기획*

- 지점별 카페 이용객 주문 및 방문 횟수를 기반으로 리워드 기준 구축 및 내용 기획
    - 성별, 나이대, 매출, 주문횟수와 내용의 2개의 카페 지점 데이터
    - 주문 횟수와 재방문 기간의 간격을 바탕으로 최상위고객, 차상위고객 분류 진행
    - 신규 카페 고객을 위한 이벤트를 통해서 15% 재방문율 증가
        - 이벤트 내용: 카페의 최애 메뉴 혹은 디저트 상품의 금액 할인을 통해서 다양한 메뉴 경험할 수 있도록 기획
    - Word2vec를 활용하여 인기있는 커피 메뉴 및 디저트 메뉴 파악
    - SQL을 활용하여 데이터 추출, Python을 활용한 데이터 추출 및 시각화, Tableau를 활용하여 매출, 성비, 지점 데이터 시각화
