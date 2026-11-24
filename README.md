# 죽은 도시의 경찰서 (DEAD PRECINCT) 한글판

PS1 스타일 레트로 서바이벌 호러 브라우저 게임 [DEAD PRECINCT](https://github.com/Bao5ye/dead-precinct)의 한국어 번역판입니다.

![대표 이미지](screenshots/cover.jpg)

## 플레이

- **온라인**: https://sigco3111.github.io/dead-precinct-ko/
- **로컬**: `index.html`을 내려받아 Chrome / Edge / Safari로 열기 (PC, 모바일 모두 가능)
- 소리는 첫 클릭 또는 키 입력 후에 나옵니다(브라우저 정책). iPhone은 무음 스위치를 해제하세요.

| 조작 | 키보드 | 모바일 |
|---|---|---|
| 전진 / 후진 | ↑ ↓ | 방향 패드 위 / 아래 |
| 제자리 회전 | ← → | 방향 패드 왼쪽 / 오른쪽 |
| 달리기 | Shift | □ (토글) |
| 조준(자동 조준) | 스페이스 누르고 있기 | R1 (토글) |
| 조사 / 문 열기 / 사격 | J 또는 엔터 | ✕ |
| 가방 | I | ○ |

플레이 타임은 약 10분: 중앙대로 → 경찰서 대홀(세이프룸) → 서쪽 사무실 → 동쪽 복도 → 무기고 → 지하 주차장 보스전.

## 스크린샷

| | | |
|---|---|---|
| ![](screenshots/street.jpg) | ![](screenshots/zombie-grab.jpg) | ![](screenshots/alarm-corridor.jpg) |
| ![](screenshots/garage-boss.jpg) | ![](screenshots/characters.jpg) | ![](screenshots/portrait.jpg) |

## 특징

- **PS1 그래픽 재현**: 320×240 렌더링, 버텍스 떨림, 15비트 디더링, 어파인 텍스처 왜곡, CRT 스캔라인과 그레인
- **탱크 방식 조작 + 고정 카메라 + 1인칭 문 열기 연출**
- **Blender 프리렌더 배경**: 10개 고정 카메라 배경을 Blender Cycles로 오프라인 렌더링 후 색보정, 실시간 3D 캐릭터를 깊이에 맞게 합성
- **분할 로우폴리 캐릭터**: 여경, 두 종류의 좀비, 오리지널 괴물 "크롤러"와 "진압자". 텍스처는 전부 코드로 픽셀 단위 생성
- **전부 실시간 합성된 사운드**: 오리지널 BGM 3곡(탐색/세이프룸/보스), 리버브, 포먼트 보컬(신음, 비명, 포효), 환경음, 심장 박동
- **호러 연출**: 죽은 척하던 좀비가 일어나고, 창문이 깨지며 습격하고, 경보 적색등이 켜지고, 전원이 나간 뒤 보스가 나타납니다

## 기술 노트

- 외부 라이브러리·에셋 없이 단일 `index.html` 하나로 동작(자체 WebGL 렌더러)
- 이 한글판은 게임 내 모든 텍스트(스토리, UI, 아이템, 지역 이름, 문서, 연출 메시지)와 코드 주석을 한국어로 번역했습니다

## 라이선스 및 원작

- 원작: [Bao5ye/dead-precinct](https://github.com/Bao5ye/dead-precinct) (MIT License, © 2026 Bao5ye)
- 원작은 한 사람과 Anthropic Claude(Fable 5.2, Opus 5.5)의 인간×AI 협업 실험으로 하루 만에 6개 버전을 거쳐 완성된 작품입니다(제작자 표기 기준)
- 이 저장소는 원작의 MIT 라이선스를 따라 수정·번역·배포하며, 원작 라이선스 전문은 [LICENSE](LICENSE)에 유지되어 있습니다
