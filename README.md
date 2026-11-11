# IRC 2026 피지컬 AI 자율용접

- 프로젝트 소개와 자료 (구성, STL 부품 파일, 학습 방법, 측정 기준): https://gawbi.github.io/irc2026-troubleshooting/project.html
- 대회 발표 (웹 슬라이드): https://gawbi.github.io/irc2026-troubleshooting/ (방향키, 스페이스, 스와이프로 넘김, F는 전체 화면)
- 이전 초안 (11/5): https://gawbi.github.io/irc2026-troubleshooting/v1.html
- 트러블슈팅 기록: https://gawbi.github.io/irc2026-troubleshooting/log.html
- 제보: [이슈 열기](https://github.com/gawbi/irc2026-troubleshooting/issues/new?template=troubleshooting.yml) (증상, 원인, 조치, 검증, 남은 일)

## 기록 추가하는 법

1. 이슈로 제보가 올라오면 사이트의 '팀원 제보'에 바로 보입니다.
2. 정리가 끝나면 `data/entries.json`에 한 항목을 추가하고 이슈를 닫습니다.

```json
{
  "id": "H8", "area": "하드웨어", "status": "해결",
  "title": "한 줄 제목",
  "symptom": "...", "cause": "...", "fix": "...", "check": "...", "next": "...",
  "image": "images/파일.jpg", "imageAlt": "그림 설명"
}
```

상태는 `확인 필요`, `보류`, `진행 중`, `해결` 중 하나입니다. 사이트에서 각각 짚색, 청동색, 보라, 파랑으로 보입니다(용접부 열변색 순서).

## 로컬에서 보기

```
python3 -m http.server -d . 8000
```
