# App_review_Crawling_EDA_Logisticregression
구글앱 크롤링 후 어플리케이션 로지스틱 회귀분석

## 개요
모바일 시장규모는 약 2천500억으로 계속 커지고 있는 상황

대기업들도 모바일 시장에 뛰어들며 본사의 유통사들을 하나로 묶는 옴니채널전략을 구사

대기업의 모바일 어플리케이션 사용시 소비자들은 어떤 서비스를 불편해 하는지 혹은 만족하는지 조사

## SSG EDA

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/1.png" height="400" width = "300px" ></p></a>

위 사진과같이 총 1879개 댓글이 달렸으며 평점은 평균 3점대 Helpful(댓글이 공감이 되면 클릭하는 컬럼)은 1댓글당 14개 정도 달린다. 하지만 helpful을 보면 편차가 심하기 때문에 좀 더 조사를 해볼 필요가 있다.

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/2.png" height="400" width = "600px" ></p></a>

2018년 12월 2019년 1월 쯤에 극단적인 Helpful이 발견 되었으며 이상치라고 판단되지 않기에 삭제안하고 진행

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/3.png" height="600" width = "1000px" ></p></a>

왼쪽 부터 2014년도에 단어 출력수 및 평균평점으로 2014년에 결제 2015년엔 쇼핑 등 각 년도별로 이슈에 대해 예측 할 수 있었다.  

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/4.png" height="500" width = "900px" ></p></a>

각년도별 평점 히스토그램으로 소비자들이 평점을 매길때 극단적으로 매기는 경우가 많다라는걸 알 수 있다.

## SSG 로지스틱 회귀 분석

2016년 데이터를 7:3으로 나누어 훈련을 진행 하였으며 테스트 결과는 아래와 같다.

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/5.png" height="200" width = "600px" ></p></a>

과소적합이 일어나면서 정확도가 많이 떨어진다. 

년도별로 훈련을 진행 했을때 과소적합이 발생해 년도를 다 합쳐서 훈련을 진행하였고 로지스틱회귀분석 결과 긍부정 단어는 아래와 같다. 

<a href="#"><p align="center"><img src= "https://github.com/riverorz/App_review_Crawling_EDA_Logisticregression/blob/main/image/6.png" height="500" width = "600px" ></p></a>


