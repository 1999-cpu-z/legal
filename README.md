# docs — 약관·정책 원본

이 폴더가 **원본**이다. 공개 게시는 별도 저장소 `legal` 에서 한다.

## 왜 저장소를 나눴나

GitHub Pages 는 **공개 저장소에서만** 무료로 동작한다(Free 플랜).
`Interior-Plat` 은 비공개라 여기서 직접 게시할 수 없다.
코드는 닫아두고 문서만 공개하기 위해 `legal` 저장소를 따로 둔다.

저장소 이름을 앱 이름(`spacer-docs` 등)으로 하지 않은 이유 —
「Spacer」는 아직 임시명이다(`Rules/10-concept-v2.md` §9).
이 URL 은 스토어 콘솔에 등록되므로 이름이 바뀌어도 그대로 써야 한다.

## 게시 절차

1. 이 폴더의 파일 전부를 `legal` 저장소 **루트**에 복사한다
   (`_config.yml` · `index.md` · `privacy.md` · `terms.md` · `community-guidelines.md`)
2. 커밋 · 푸시
3. `legal` 저장소 → Settings → Pages → Source = `main` / `(root)`
4. 1~2분 뒤 아래 주소가 열리는지 확인한다

```
https://1999-cpu-z.github.io/legal/privacy/
https://1999-cpu-z.github.io/legal/terms/
https://1999-cpu-z.github.io/legal/community-guidelines/
```

## ⚠ 수정할 때

**여기를 고치고 `legal` 로 복사한다.** 반대로 하면 원본이 갈라진다.
URL 을 바꿀 일이 생기면 `lib/config/legal_config.dart` 한 곳만 고치면 앱에 반영된다.

## ⚠ 방침을 갱신해야 하는 시점

개인정보처리방침은 **실제로 수집하는 항목만** 적혀 있다.
`spaces` 테이블에는 `camera_intrinsics` · `capture_position` · `depth_map_url` ·
`color_profile` · `ceiling_height` · `area_pyeong` 컬럼이 있지만 앱이 채우지 않는다.
**이 값들을 실제로 수집하기 시작하면 방침을 먼저 갱신해야 한다.**
