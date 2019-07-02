# Fastcampus DSS+1 Classification project

[Walmart Recruiting: Trip Type Classification](https://www.kaggle.com/c/walmart-recruiting-trip-type-classification)

월마트에서 자체적으로 분류한 38개의 고객 유형이 있고, 고객의 구매 이력만을 보고 고객 유형을 예측하는 분류문제입니다. 

learning rate를 0.02, max depth를 30으로 setting하고 lgbm으로 학습시킨 부스팅 모델이 가장 성능이 좋았습니다. accuracy는 77%입니다. 

feature importance는 물건을 몇개 샀는지 측정한 scan count가 가장 높았고, 그 뒤로는 EDA 과정을 통해 생성한 feature들이 뒤를 이었습니다. (물건의 대분류, 요일, 바코드 길이 등)

classification report를 분석해 보았을 때, 잘 분류하지 못하는 특정 class가 있었습니다. 이는 EDA 과정에서 살펴보았던것처럼 고객 유형 하나가 한 종류의 상품만을 구매하지 않기 때문이라고 유추해볼 수 있습니다.
