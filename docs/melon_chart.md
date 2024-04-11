
# 프로젝트 개요
데이터 애널리스트 트랙 부트캠프 수강 기간 중, 2명의 팀원과 같이 멜론의 곡, 가수, 앨범 정보 페이지와 시대별 차트 페이지를 스크래핑 하여, 2000년 부터 2019년 까지의 음원 차트 데이터를 분석.

Python 스크립트를 이용하여 스크래핑한 정보를 로컬 SQL 서버에 저장한 뒤 MySQL Workbench 프로그램을 사용하여 쿼리를 실행해 원하는 통계 정보를 얻어냄.

# 개인 기여도 및 배운 내용
- 팀 인원: 3명
- 개인 기여도: 40%
- 담당 파트: 데이터베이스 ERD 설계와 차트 페이지에서 차트에 수록된 곡, 가수, 앨범 페이지로 자동으로 이동하며 각 페이지의 정보를 수집하는 코드 담당.
- 보안할 점: many-to-many 관계를 표현하기 위해 SONG_SINGER, ALBUM_SINGER 테이블을 추가한 건 좋았지만, ALBUM_SONG 테이블은 one-to-many 관게를 가지고 있기 때문에 Foreign Key를 사용하면 추가적인 테이블 사용이 없어도 되었을텐데 프로젝트 초기에 이 부분을 간과해서 아쉬웠다.

# 사용 기술
- Python
- Selenium, BeautifulSoup
- MySQL, MySQL Workbench

# 참고 링크
- [전체 코드베이스](https://github.com/jsh318900/mini_project_1_team_3/tree/master)
- [곡, 가수, 앨범 페이지 스크래핑 코드 (담당 파트)](https://github.com/jsh318900/mini_project_1_team_3/blob/master/python/webscraper/page_scraper.py)
- [SQL 테이블 생성 코드 (담당 파트)](https://github.com/jsh318900/mini_project_1_team_3/blob/master/sql/create_table.sql)
- [분석 쿼리 결과 및 발표 자료 pdf](https://github.com/jsh318900/mini_project_1_team_3/blob/master/%EB%B0%9C%ED%91%9C%EC%9E%90%EB%A3%8C.pdf)
