# 꼬마 게임 모음

4·5살 아이와 함께 하는 모바일 웹 게임 모음. 게임마다 폴더 하나, 폴더 안에 `index.html` 한 파일.

- 게임 목록: https://ksloo6-svg.github.io/kids-games/
- 눈굴리기 대작전: https://ksloo6-svg.github.io/kids-games/snowball/
- 숫자 대장: https://ksloo6-svg.github.io/kids-games/numbers/
- 구멍 먹보: https://ksloo6-svg.github.io/kids-games/hole/

## 새 게임 추가
1. `게임이름/` 폴더를 만들고 `index.html`(필요하면 아이콘·manifest) 넣기 — 경로는 모두 상대경로로
2. 루트 `index.html`의 `.shelf`에 카드(`<a class="game" href="게임이름/">`) 추가
3. localStorage 키는 게임마다 고유 접두사 사용(예: `snowball-`). 모든 게임이 같은 출처(ksloo6-svg.github.io)를 공유함
