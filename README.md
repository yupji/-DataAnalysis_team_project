# 🙌목적
- 영화 제작사 측에서 여러가지 데이터를 보고 흥행 요소에는 어떤 것들이 있는지 파악 가능 
- 데이터 수집(크롤링) 및 정제, 시각화를 함으로써 수업시간에 배웠던 내용 복습 및 실력 향상

# ❓타겟 사이트 선정
- 역대 박스오피스 관객 수 기준 상위 200위를 보여주는 사이트인 영화권입장권 통합전산망(https://www.kobis.or.kr/kobis/business/main/main.do)으로 선정
- 한국 영화만 크롤링 기법으로 데이터 수집

# 😀참여인원
- [1조]
- 지승엽 : 데이터 크롤링, 시각화 및 분석, 보고서 제작
- 이용희 : 타겟선정, 데이터 크롤링, ppt 제작

# 👆데이터 크롤링
## 수집할 데이터 형태
- 영화 목록
![image](https://user-images.githubusercontent.com/125621591/229723475-ad0dbc0b-9649-487a-a259-ca91149c9ae9.png)

- 각 영화 내부 정보 형태
![image](https://user-images.githubusercontent.com/125621591/229723976-c0333a01-26b7-4e96-8646-dc77be1f45b9.png)
  - 각 영화의 링크를 반복으로 클릭해서 정보 추출(장르, 상영시간, 관람 등급, 감독, 배우) 등
  
## 수집한 데이터를 데이터프레임으로 변환
- 컬럼 : title, opening_date, sales, attendance, screen, show_count, genre, runtime, content_rating, director, actor, distributor

![image](https://user-images.githubusercontent.com/125621591/229724982-3f92bac2-3d8c-46fa-b23d-2ad7564e7836.png)
![image](https://user-images.githubusercontent.com/125621591/229725046-f27d8aed-ab84-4b65-9a9c-6b3107ffe7ca.png)

# 👀데이터 시각화
## 첫번째 요소 : 3번 이상 출연한 배우들(100명)
<img src="https://user-images.githubusercontent.com/125621591/229726690-ec70aed8-35a4-41ae-b269-2ea60519ac68.png" width="500" height="400"/>

## 두번째 요소 : 상위 200위 영화 중 3개 이상 만든 감독
![image](https://user-images.githubusercontent.com/125621591/229728135-81baed04-a47d-447d-adae-998060d51474.png)

## 세번째 요소 : 장르별 비율
<img src="https://user-images.githubusercontent.com/125621591/229728559-57df8e1e-7a70-435d-87ce-ecb73e8d18e1.png" width="400" height="400"/>

## 네번째 요소 : 관람 등급
![image](https://user-images.githubusercontent.com/125621591/229728763-dc454ff3-d05a-4a52-9c32-a2a090d01934.png)

## 다섯번째 요소 : 배급사
![image](https://user-images.githubusercontent.com/125621591/229728984-44bf39ed-a5df-4f7c-9643-d8d98615bd74.png)
- 4대 배급사가 배급의 대부분을 담당하고 있음

## 여섯번째 요소 : 개봉시기(월별)
![image](https://user-images.githubusercontent.com/125621591/229729400-29397050-a092-4baf-91f5-ae5c36be45da.png)
- 연말연시, 가정의 달인 5월, 여름휴가기간인 7,8월에 관객 수가 많은 편

# 👨‍🎓결론 및 기대효과
- 결론 : 데이터를 수집하고 정제하여 분석 및 시각화를 해보니 상대적으로 유의미한 데이터(장르, 배급사, 관람 등급 등)도 있는 반면에 의미가 있을 것이라고 예상해 추출한 데이터(상영 길이 등)가 무의미한 경우도 존재했다.
- 기대효과 : 제작사 입장에서 이 데이터를 보고 영화를 제작할 때 어떤 요소에 더 가중치를 줘야하는지 알 수 있을 것이다
