# 5th L.point_bigdata_competiton

* 진행 과정
  
  * [2018-12-25] [EDA](https://github.com/miniii222/5th_L.point_bigdata_competiton/tree/master/EDA)
  * [2018-12-26] 아이디어 회의 및 스케줄 조정
    - product 데이터 : []괄호 찾아서 지움, PD_ADD_NM column 삭제 -> 01-2Product.csv
  * [2018-12-27] [시각화 및 EDA](https://github.com/miniii222/5th_L.point_bigdata_competiton/tree/master/EDA)
    - 데이터가 커서 r로 부르면 잘 안 불러짐
    - python은 익숙치 않아서 큰 일
  * [2018-12-28] [column 생성 및 데이터 처리](https://github.com/miniii222/5th_L.point_bigdata_competiton/tree/master/EDA)
    - product 데이터 : hits=1 인 경우 삭제 -> drop_product.csv
    - master 데이터 : [대대분류 분류 추가](https://github.com/miniii222/5th_L.point_bigdata_competiton/blob/master/EDA/EDA_02.master.ipynb)
    - session 데이터 : 주말효과 -> new_session.csv
  * [2018-12-30] [clustering]
    - mixed-type SOM 참고 논문 [link:](https://www.sciencedirect.com/science/article/pii/S1568494612001731)
  * [2019-01-01]
    - 20대 여성에 대해서 의미있는 것 같기도 하고...
    - 상품군별 유의미한 변수를 알기 위한 모델링 (elastic net, ols)
    - 전체 데이터를 이용한 clustering
  * [2019-01-03]
    - clustering을 위해 merge한 데이터 : merged_data.csv
    - 주말효과 넣은 clustering
    - 새로운 데이터가 들어갔을 때, cluster간의 거리와 비율을 이용하여 index 출력하는 
  * [2019-01-04]
    - clustering 후, 비율처리 하는 것 수정 예정
    - search1 파일에서 konlpy 이용하여 브랜드이름 뽑을 
  * [2019-01-08]
    - search1 데이터 : [파일에서 브랜드 칼럼 저장](https://github.com/miniii222/5th_L.point_bigdata_competiton/blob/master/text/Search_extract_brand.ipynb) -> Search1_brand.csv
  * [2019-01-09]
    - 클러스터링의 문제점 발견 -> 절망적!
    - 브랜드 칼럼 + 상품명 칼럼
    - 날씨 데이터
  * [2019-01-10]
    - 네이버 데이터랩 활용하는 방안 -> 선호지수 및 트랜드 예측
    - 주요 상품군별 OLS, elastic net 모델링
  * [2019-01-11]
    - 네이버 데이터랩 데이터 칼럼 
    - 상관관계 분석 후 선호지수 생성
  * [2019-01-14]
    - 대대분류 별 lstm 
