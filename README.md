# scraping_ncpssd
国家哲学社会科学文献中心 문헌 서지 정보 수집 코드(js)<br>
Scraping Bibliographic Information from National Center for Philosophy and Social Sciences Documentation<br>

\<기본 사항\>
- 사용 방법: www.ncpssd.cn 에서 검색 후 개발자도구-콘솔에 직접 입력<br>
- 시행 동작: 검색 결과를 마지막 페이지까지 순회하며 수집 후 xml 파일로 저장<br>
- 사용자 입력: 코드 실행시 최대 순회 횟수(기본값: 100)와 저장 파일명 요소(기본값: list) 입력 필요<br>
- 저장 파일명: articles_(입력한 저장 파일명 요소)_(저장 날짜).xml
<br>

\<예시 파일\>
- articles_krzzyj_2025-08-18.xml : 抗日战争研究(1991-2025), 中国社会科学院近代史研究所<br>
- articles_jdsyj_2025-08-18.xml : 近代史研究(1979-2025),  中国社会科学院近代史研究所

XML 파일은 \<articles\> 루트 아래에 여러 개의 \<article\> 단위로 구성.  
각 \<article\>은 \<title\>, \<journal\>, \<year\>, \<issue\>, \<authors\>, \<funding\>, \<abstract\>, \<keywords\>, \<impact\> 등의 태그로 구성.
