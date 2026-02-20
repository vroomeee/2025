# 11반 롤링페이퍼

GitHub Pages에 바로 올릴 수 있는 정적 웹페이지입니다.

## 구성
- 2x2 그룹 배치 (총 4개 조)
- 조마다 4자리 (총 16자리)
- 좌석 클릭 시 해당 학생 메시지 팝업 표시
- 조 이름(백범조, 김구조, 아인슈타인조, 간디조)을 책상 중앙에 표시

## 메시지/이름 수정
`index.html` 하단의 `teamData`만 수정하면 됩니다.

```js
const teamData = [
  {
    groupName: "백범조",
    seats: [
      { student: "학생 1", note: "메시지" },
      ...
    ]
  },
  ...
];
```

- `groupName`: 조 이름
- `student`: 좌석에 표시될 이름
- `note`: 클릭했을 때 보이는 롤링페이퍼 문구

## GitHub Pages 배포
1. 이 폴더를 GitHub 저장소에 push
2. 저장소 `Settings` → `Pages`
3. `Build and deployment`에서 `Deploy from a branch` 선택
4. `Branch`: `main`(또는 `master`) / `/ (root)` 선택 후 저장
5. 1~3분 뒤 발급된 주소로 접속
