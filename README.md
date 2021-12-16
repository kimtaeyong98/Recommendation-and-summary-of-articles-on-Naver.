# Recommendation-and-summary-of-articles-on-Naver.
네이버 기사를 크롤링 하여 사용자가 원하는 토픽을 가장 잘 설명하는 기사를 찾고 요약해주는 로직입니다.

(konlpy, BeautifulSoup, pororo 이용 )

크롤링 대상: 언론사 별 조회수 상위 20개 기사

마지막 코드 동작 확인일 : 2021-06-15

<동작과정>

![image](https://user-images.githubusercontent.com/63800086/146407976-e82da776-febc-4f17-b2cf-ab34a4e5c250.png)


<크롤링 결과>

![image](https://user-images.githubusercontent.com/63800086/146408260-2df18996-8a1e-4325-8864-0448e1d3f996.png)




<전처리>

![image](https://user-images.githubusercontent.com/63800086/146408638-749dfaa7-fbed-4783-92dc-a055ebe801a8.png)



<사용자 입력 1단계 - 분야 선택> - 사용자가 선택 분야의 데이터만 추출 및 토픽 추출

![image](https://user-images.githubusercontent.com/63800086/146408835-4e88f814-3cd8-4973-84bf-c1ed5b1c881e.png)



<사용자 입력 2단계 - 토픽 입력> - 사용자가 선택한 토픽에 대한 기사 데이터만 추출

![image](https://user-images.githubusercontent.com/63800086/146408984-b8c8b1f7-fb42-487f-9ed2-fc62d09ba650.png)



<알고리즘 적용> - 2단계 까지 추출된 기사 데이터를 이용하여 알고리즘 적용

알고리즘1 : 카운트 기반

알고리즘2 : Apriori




<기사 추출>

두 알고리즘으로 추출된 결과값의 정규화 평균이 가장 높은 기사를 선택




<기사 요약>

카카오브레인의 pororo 모델을 이용하여 기사 요약


<결과 예시>


![image](https://user-images.githubusercontent.com/63800086/146410382-51b6cc70-41d2-4e97-9743-61b02b659479.png)

: 6/11일에 "사회" 분야에서 "건물"이란 키워드가 핫토픽인 된 이유는 건물 붕괴 사고 때문임을 알 수있다.




