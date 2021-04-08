# 통합
### 팀 전체 의견을 통합  

## Data set
[소상공인시장진흥공단_상가(상권)정보](https://www.data.go.kr/data/15012005/fileData.do), [seoul_municipalities_geo_simple.json](https://github.com/CodeDiary18/Commercial-Districts-Analysis/blob/main/data/seoul_municipalities_geo_simple.json), [TL_SCCO_SIG.json](https://github.com/CodeDiary18/Commercial-Districts-Analysis/blob/main/data/TL_SCCO_SIG.json)


## File introduction
### [스타벅스_메가커피 입지비교.ipynb](https://github.com/CodeDiary18/Commercial-Districts-Analysis/blob/main/%ED%86%B5%ED%95%A9/%EC%8A%A4%ED%83%80%EB%B2%85%EC%8A%A4_%EB%A9%94%EA%B0%80%EC%BB%A4%ED%94%BC%20%EC%9E%85%EC%A7%80%EB%B9%84%EA%B5%90.ipynb)
#### 요약
* data라는 폴더에서 분석하고 싶은 도시의 스타벅스와 메가커피 매장에 대한 분석


#### 전처리
* data라는 폴더에서 분석하고 싶은 도시의 csv파일을 불러와서 데이터프레임으로 저장하고 필요없는 열을 제거함
* 불러온 데이터프레임에서 스타벅스와 메가커피에 대해서 다시 데이터를 정리해서 저장


#### 분석
* 막대그래프
  * 브랜드명 
* 산점도(scatter): 브랜드명별로 산점도 찍기
* groupby와 pivot_table로 구별 스타벅스, 메가커피 매장 수 구하기
* 지도
  * folium 활용해 스타벅스 메가커피 카페 매장 전체 분포 확인
  * GeoJSON 파일 로드 후 스타벅스, 메가커피 메장 수 각각 확인
 


### [카페 상권분석.ipynb](https://github.com/CodeDiary18/Commercial-Districts-Analysis/blob/main/%ED%86%B5%ED%95%A9/%EC%B9%B4%ED%8E%98%20%EC%83%81%EA%B6%8C%EB%B6%84%EC%84%9D.ipynb)
#### 요약
* data라는 폴더에서 분석하고 싶은 도시와 분석하고 싶은 카페 브랜드 2개를 입력받고 그에 대한 매장에 대한 분석


#### 전처리
* data라는 폴더에서 분석하고 싶은 도시의 csv파일을 불러와서 데이터프레임으로 저장하고 필요없는 열을 제거함
* 불러온 데이터프레임에서 입력받은 커피 브랜드 2개에 대해서 다시 데이터를 정리해서 저장


#### 분석
* 막대그래프
  * 도시의 점포수 비교
  * 시군구별 점포수

* 산점도(scatter) : 매장 위치를 위도, 경도로 산점도 찍기
  * 두개의 브랜드
  * 각각 브랜드

* 지도
  * 지도에 circlemarker로 매장 위치 시각화
  * choropleth로 자치구별 매장수 시각화
