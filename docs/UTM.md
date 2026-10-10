# 유입 경로(UTM) 링크 모음

사이트 주소 끝에 꼬리표(`?utm_source=...`)를 붙여서 나눠 주면, 그 링크로 들어온 손님이 견적 문의를 남겼을 때
관리자 페이지(/admin)에 **어디서 보고 왔는지**가 함께 표시된다.

- 꼬리표는 30일 동안 기억된다. 손님이 QR로 들어왔다가 며칠 뒤 다시 와서 문의해도 "명함 QR"로 남는다.
- 꼬리표 없이 네이버·구글 검색에서 들어오면 "네이버 (검색·블로그)", "구글 검색"으로 자동 표시된다.
- 아무 정보가 없으면 "직접 방문"(주소를 직접 입력했거나 즐겨찾기).
- 사이트 주소가 바뀌면(예: 연산메탈.com 연결) 아래 링크의 앞부분만 바꾸면 된다.

## 바로 쓰는 링크

| 어디에 쓰나 | 링크 | 관리자 화면 표시 |
|---|---|---|
| 명함 QR | https://younsanmetal-site.vercel.app/?utm_source=namecard&utm_medium=qr | 명함 QR |
| 종합 카탈로그 QR | https://younsanmetal-site.vercel.app/?utm_source=catalog&utm_medium=qr | 카탈로그 QR |
| 카카오톡으로 보내기 | https://younsanmetal-site.vercel.app/?utm_source=kakao&utm_medium=message | 카카오톡 메시지 |
| 지인·거래처 소개용 | https://younsanmetal-site.vercel.app/?utm_source=referral&utm_medium=message | 지인 소개 메시지 |
| 네이버 블로그 글 | https://younsanmetal-site.vercel.app/?utm_source=blog&utm_medium=social | 블로그 SNS |

## 직접 만들 때

`사이트주소/?utm_source=어디서&utm_medium=어떤방식&utm_campaign=행사이름`

- `utm_source` (필수): 어디서 — namecard, catalog, kakao, referral, blog, naver, instagram
- `utm_medium`: 어떤 방식 — qr, message, social, print, cpc(유료 광고)
- `utm_campaign` (선택): 행사·기간 이름. 영어·숫자로. 예: `2026-fall`, `nonghyup-expo`
- 위 목록에 없는 값도 쓸 수 있다. 관리자 화면에는 적은 그대로 보인다.
