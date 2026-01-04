⚾️ LG Twins Data Analysis Project

LG 트윈스 데이터 분석원을 목표로 하는 KBO 데이터 수집 및 시각화 프로젝트입니다. 단순한 기록 확인을 넘어, 차단된 데이터를 확보하고 전처리하여 인사이트를 도출하는 과정을 담았습니다.

1. 프로젝트 개요
  목표: KBO 공식 홈페이지 데이터 수집 자동화 및 LG 트윈스 타자 성적 분석

  동기: 2026년 KBOP 신입사원 채용 대비 및 데이터 분석 역량 강화

  기간: 2026.01 ~ 진행 중

2. 기술 스택 (Tech Stack)
  Language: Python 3.11

  Library: Selenium, Pandas, Seaborn, Matplotlib, undetected-chromedriver

  Tool: VS Code, Jupyter Notebook (.ipynb), GitHub

3. 주요 수행 내용
  🛠 데이터 수집 (Data Collection)
    KBO 공식 홈페이지 크롤링: Selenium을 활용하여 동적 페이지 데이터 수집

  보안 이슈 해결 (Troubleshooting):

    문제: 일반적인 크롤링 시 KBO 서버의 Anti-bot 정책으로 인한 error.html 리다이렉션 발생

    해결: undetected-chromedriver를 사용하고, 수동 세션 확보와 driver.page_source 파싱 기법을 결합하여 데이터 확보 성공

🧹 데이터 전처리 (Data Preprocessing)
  타입 변환: 문자열(object)로 수집된 기록 데이터를 수치형(float, int)으로 일괄 변환

  결측치 처리: 기록이 없는 항목은 0으로 채우고, 통계적 신뢰성을 위해 10타석(PA) 미만 선수는 분석에서 제외

📊 시각화 및 인사이트 (EDA)
  타율(AVG) 순위 시각화: Seaborn을 활용하여 팀 내 주요 타자들의 타격 생산력을 막대 그래프로 구현

  가독성 개선: 한글 폰트 설정 및 x축 라벨 회전 처리를 통해 시각적 완성도 제고

4. 분석 결과
  2025 시즌 초반 신민재, 문성주 등 주축 타자들의 높은 타율 유지 확인

5. 향후 계획
  투수 기록 수집 및 평균자책점(ERA) 분석 추가

  OPS, wRC+ 등 세이버메트릭스 지표 직접 산출 및 시각화

  잠실 야구장 파크팩터를 고려한 타자 성적 보정 분석
