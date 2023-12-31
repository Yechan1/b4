# [B4] Monthly Project I



- 역할 분담 표

| 이름 | 역할 |
| --- | --- |
| 이동기 | EDA Team, 노션정리 |
| 정희상 | EDA Team |
| 김성식 | EDA Team |
| 김예찬 | 잡일 |

- 결과물
    
    [노션 페이지](https://www.notion.so/93fc5a1ebd7e481ab2568f4034142633?v=84eccd451b14445f973504f67314aacd)
    

- 데이터 셋
  
  [Real Estate DataSet](https://www.kaggle.com/datasets/arslanali4343/real-estate-dataset)


  
- 데이터 셋 변수 설명

  - CRIM : 지역의 범죄율
  - ZN : 지역에서 25,000 평방 피트가 넘는 주택지 비율
  - INDUS : 지역에서 상업적으로 사용되지 않는 농지 면적
  - CHAS : 지역이 Charles 강과 접하고 있으면 1, 아니면 0
  - NOX : 지역의 산화질소 농도
  - RM : 가구당 평균 방 수
  - AGE : 1940년 이전에 지어진 주택 비율
  - DIS : 5개의 보스턴 고용 센터와의 거리에 따른 가중치
  - RAD : Radial 고속도로 접근성 지수
  - TAX : 1만 달러당 재산세
  - PTRATIO : 지역의 학생수와 교사수의 비율
  - B : 지역의 흑인 지수  1000(𝐵𝑘−0.63)2 | 여기서 지역별 Bk는 흑인의 비율
  - LSTAT : 지역의 빈곤층 비율
  - MEDV : 자가 소유자의 주택 중앙값(중위값)을 천 달러 단위로 나타낸 것



- 분석해볼 주제

  - 강과 재산세 혹은 주택의 중앙값
  - 고속도로 접근성과 주택가격
  - 지역 범죄율과 주택 가격
 
  
- EDA 방향성

  - 기본적으로 Y값은 집값(MEDV)로 잡고 X를 변형시켜가며 plot을 하되 scatterplot을 해 본 결과 X가 범주형 자료에 가까우면 KDEplot, boxplot등을 사용하고, 연속형 자료에 가까우면 scatterplot과 함께 중앙값으로 X를 분류한 후 KDEplot, boxplot을 해 범주형 자료의 KDEplot과도 비교할 수 있도록 한다. (비례하는지 반비례하는지는 corr만 봐도 알 수 있으니 우리는 디테일하게 어떻게 분포되어있는지에 주목해야한다.)
 

- EDA 결론
  - 집값과 비례하는 요인으로는
    - 1. 방의 수
    - 2. 25000 평방 피트 넘는 주택지 비율
    - 3. 흑인 지수
    - 4. 고용 센터와의 거리
    - 5. 찰스 강과 접함 여부 순으로 강했고

  - 반비례하는 요인으로는
    - 1. 빈곤층 비율
    - 2. 사용되지 않는 농지 면적
    - 3. 1만 달러당 재산세
    - 4. 학생교사비율
    - 5. 산화질소 농도
    - 6. 고속도로 접근성
    - 7. 범죄율
    - 8. 1940년 이전에 지어진 주택 비율 순으로 강했다.

  - 의외의 분석이라하면 흑인 지수와 1만달러당 재산세, 고속도로 접근성 등이 있다.
