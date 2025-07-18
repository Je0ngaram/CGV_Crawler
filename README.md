
# 🎬 CGV 영화 리뷰 크롤링 및 감성 분석 프로젝트

CGV Crawler는 CGV 공식 웹사이트에서 현재 상영 중인 영화들의 리뷰를 수집하고, 리뷰 내용을 기반으로 감성 분석(긍정 / 부정 / 중립)을 수행하며 다양한 시각화 결과를 생성하고 저장하는 시스템입니다.  

---

## ✅ 주요 기능

- ✅ CGV 영화 리뷰 자동 크롤링 (Selenium)
- ✅ 각 영화 리뷰들을 긍정/부정/중립으로 감성 분류
- ✅ 감성 분석 결과를 시각화 (파이차트, 막대그래프, 워드클라우드)
- ✅ 각 영화별 리뷰를 개별 CSV로 저장하고 전체 통합본 생성
- ✅ 자동 폴더 생성 및 중복 방지 번호 붙이기 기능

---

## 🛠 사용 기술 및 환경

- 언어: Python 3.x
- 웹 크롤링: Selenium
- 데이터 처리: Pandas
- 감성 분석: 키워드 기반 룰
- 시각화: matplotlib, wordcloud
- 실행 환경: Jupyter Notebook

---

## 🧠 감성 분석 기준

- **긍정 키워드** 예시: '좋다','재밌다','감동','최고','웃기다','흥미진진','꿀잼','감명', '귀엽', '참 잘', '따뜻'
- **부정 키워드** 예시: '별로', '최악', '실망', '노잼', '지루했어요', '망작', '형편없다', '재미없음','진부'

---

## 📊 시각화 예시

### 🎬 1. 전체 리뷰 통합 영화별 감성 분포
![영화별 감성 분포](https://github.com/Je0ngaram/CGV_Crawler/blob/main/image/%EC%82%AC%EC%A7%841.png)

---

### 🌈 2. 전체 리뷰 워드클라우드
![워드클라우드](https://github.com/Je0ngaram/CGV_Crawler/blob/main/image/%EC%82%AC%EC%A7%842.png)

---

### 📊 3. 전체 리뷰 감성 분포 막대 그래프
![감성 막대그래프](https://github.com/Je0ngaram/CGV_Crawler/blob/main/image/%EC%82%AC%EC%A7%843.png)

---

### 🥧 4. 전체 리뷰 감성 분포 원형 그래프
![감성 원형그래프](https://github.com/Je0ngaram/CGV_Crawler/blob/main/image/%EC%82%AC%EC%A7%844.png)

---

### 🧠 5. 모든 영화 리뷰 전체 통합 감성 분포
![전체 통합 감성 원형](https://github.com/Je0ngaram/CGV_Crawler/blob/main/image/%EC%82%AC%EC%A7%845.png)

---

## 📌 실행 방법 요약

1. 필수 패키지 설치
```bash
pip install selenium pandas matplotlib wordcloud
```

2. 크롬드라이버 설치 후 경로 지정

3. Jupyter에서 `CGV_Crawling.ipynb` 실행
-셀 순서대로 위에서 아래로 하나씩 실행

---

## ❕ 느낀 점

리뷰 데이터는 형태가 일정하지 않고, 종종 공백이나 특수문자, 짧은 문장 등이 포함되어 있어서 정제와 전처리가 중요함을 느꼈다.

영화별 긍/부정/중립 분포 막대 그래프, 전체 리뷰 감성 원형 그래프, 워드클라우드 등을 통해 다양한 분석 결과를 표현할 수 있었다.
