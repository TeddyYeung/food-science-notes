# food-science-notes

요리 과학을 5살도 알게 그림으로 설명하는 작은 사이트다. 책 『더 푸드 랩』 대신 무료 영상과 글로 원리를 배운다.

- 사이트: https://teddyyeung.is-a.dev/food-science-notes/
- 하위 도메인 `food.teddyyeung.is-a.dev`는 is-a.dev 승인 뒤에 연결한다.

## 페이지

| 파일 | 내용 |
|---|---|
| `index.html` | 목차 |
| `osmosis.html` | 김치 속 삼투압. 출처: [Beyond Words 영상](https://youtu.be/hUfKdDW4Wpw) |
| `wilting.html` | "숨이 죽는다"는 말 |
| `vegetable-water.html` | 채소의 수분, 요리별 물 빼기, 볶음이 물러지는 이유 |
| `study.html` | 요리 과학 영상과 글, 보는 순서 |
| `foodlab-map.html` | 켄지 로페즈-알트 영상과 Food Lab 칼럼 중 원리 설명 85개 |
| `mcgee.html` | 해럴드 맥기 『음식과 요리』 대신 읽을 요약 연재 11개, 서평 3개, 영문 요약 3개, 영상 4개. 항목마다 5살 버전 |

## 데이터

`data/kenji-youtube-videos.tsv`: [@JKenjiLopezAlt](https://www.youtube.com/@JKenjiLopezAlt/videos) 채널 영상 638개 (id, 길이, 조회수, 제목). 2026-10-26 기준.

## 로컬에서 보기

```bash
python3 -m http.server 8765
```

## 참고

- Food Lab 칼럼 전체 353개 목록은 저장하지 않았다. Serious Eats가 스크립트 접근을 막아서 브라우저에서만 읽었다.
- `foodlab-map.html`의 항목 85개에 모두 5살 버전 설명을 붙였다. 설명마다 비유 문장이 1개 이상 있다. 주제마다 비유 그림(SVG)도 1개씩 있다.
- `study.html`의 채널 8개에도 5살 버전 한 줄을 붙였다. 그림은 3개다.
- 글의 5살 버전은 Serious Eats 본문을 브라우저에서 읽고 썼다. 영상의 5살 버전은 `yt-dlp`로 받은 영어 자막 전체를 읽고 썼다 (31개 모두 자막 있음).
- 항목마다 ‘더 알아보기’ 인사이트가 2~3개 있다 (`MORE`, 모두 254개). 실험 결과, 숫자, 원리, 흔한 실수를 같은 원문에서 뽑았다.
- `mcgee.html`의 5살 버전은 블로그 글과 서평 본문, 영상 자막(`yt-dlp`)을 읽고 썼다. 캐나다삼촌 영상에는 이 책이 나오지 않는다.
- 채소 수분 비율은 대략적인 값이다.
