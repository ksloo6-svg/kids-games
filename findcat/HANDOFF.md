# 숨은 고양이 찾기 (findcat)

Find The Cat 2 방식 숨은그림찾기. 단일 `index.html`, 그림은 모두 코드로 그린 SVG.

- 장면 8가지가 레벨마다 돌아가며 나옴: 아이 방, 부엌, 마당, 바닷가, 숲속, 우주정거장, 눈 마을, 공원 (`THEMES`).
- 레벨 번호가 랜덤 시드라 같은 레벨은 항상 같은 그림 (`buildLevel`). 레벨이 오를수록 장면이 넓어지고 물건이 많아지고 고양이가 작아짐 (`levelSpec`).
- 고양이 수: 3마리부터 2레벨마다 +1, 최대 12.
- 숨는 방법 (`placeCat`): top(물건 위에 앉기), peek(물건 뒤에서 빼꼼), side(옆으로 반만), lie(위에서 잠), tail(꼬리만). 레벨마다 쓰는 방법이 늘어남 (`modesFor`).
- 게임오버: 빈 곳 누르면 하트 -1 (3개), 하트 0 또는 시간 끝 → 다시 하기. 게임오버 때 못 찾은 고양이를 노란 원으로 보여줌.
- 보상: 깨면 코인 10 + 남은 하트×5, 처음 깬 레벨이면 힌트 +1. 힌트는 코인 30으로 구매. 시작 힌트 2개.
- 조작: 탭(찾기), 한 손가락 끌기(이동), 두 손가락(확대), ＋ － 버튼, PC는 휠.
- 저장 키: findcat-max, findcat-level, findcat-coins, findcat-hints, findcat-sound.
- 디버그: `window.__debug` (startLevel, tapWorld, lev, game), 아이콘은 `__iconSVG()` 로 생성.
