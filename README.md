# ShortForm 한글 글꼴 모음

ShortForm 앱에서 자막·제목에 쓸 수 있도록, **다시 배포해도 되는 무료 한글 글꼴**을 모아 둔 곳입니다.
앱은 이 저장소의 파일을 jsDelivr 로 받아 씁니다.

```
https://cdn.jsdelivr.net/gh/sunwoojune/shortform-fonts@<커밋>/manifest.json
https://cdn.jsdelivr.net/gh/sunwoojune/shortform-fonts@<커밋>/fonts/<글꼴 id>/<파일 이름>
```

주소에는 늘 **커밋 해시**를 붙여 씁니다. 그래야 파일이 바뀌지 않고, `manifest.json` 의 sha256 으로 받은 파일이 맞는지 확인할 수 있습니다.

## 꼭 알아 둘 것

- **글꼴마다 라이선스가 따로 있습니다.** 각 폴더의 `LICENSE`(약관 원문)와 `SOURCE.md`(공식 받은 곳·받은 날·sha256·만든 곳)를 보세요.
- 이 저장소의 글꼴은 모두 **상업적으로 써도 되고, 영상 자막에 써도 되고, 다시 배포해도 되는 것**만 골랐습니다(2026-10-06 공식 약관 확인).
- 글꼴 파일은 **공식 배포처에서 받은 그대로**입니다. 이름도 내용도 바꾸지 않았습니다(OFL 예약 이름 조항, 에스코어 「파일 수정 금지」 조항).
- 글꼴 파일 **자체를 파는 것은 어느 글꼴도 안 됩니다.** 이 저장소도 팔지 않습니다.
- 글꼴 저작권은 각 제작사에 있습니다. 이 저장소는 배포만 돕습니다.

## manifest.json

맨 위 `manifest.json` 에 파일마다 한 줄씩 들어 있습니다.

| 칸 | 뜻 |
|---|---|
| `id` | 글꼴 묶음 id(폴더 이름) |
| `name` | 한국어 이름 |
| `family` | 글꼴 파일 안 이름(name 테이블 1번 칸) — 자막(ASS)에서 이 이름으로 부릅니다 |
| `style` / `weight` | 굵기 이름 / 파일 안 굵기 숫자(OS/2) |
| `file` | 저장소 안 경로 |
| `sha256` / `size` | 파일 해시 / 바이트 크기 |
| `license` | 라이선스 이름 |
| `source` | 공식 받은 곳 |
| `category` | 고딕·명조·손글씨·디자인 |
| `maker` | 만든 곳 |
| `hangul` | 파일에 든 완성형 한글 글자 수(11172 이면 전부, 2350·2780 이면 자주 쓰는 글자만) |

- 나눔바른고딕은 보통·굵게가 family 이름이 같고 style 만 다릅니다(Regular / Bold).
- 파일 하나는 모두 20MB 아래입니다(jsDelivr 한 파일 한도).

## 들어 있는 글꼴 (69벌, 파일 100개)

| 이름 | 폴더 | 분류 | 파일 수 | 굵기 | 라이선스 |
|---|---|---|---|---|---|
| 나눔스퀘어 | `fonts/nanum-square/` | 고딕 | 3 | Regular, Bold, ExtraBold | OFL-1.1 |
| 나눔스퀘어라운드 | `fonts/nanum-square-round/` | 고딕 | 3 | Regular, Bold, ExtraBold | OFL-1.1 |
| 나눔스퀘어 네오 | `fonts/nanum-square-neo/` | 고딕 | 4 | Regular, Bold, ExtraBold, Heavy | OFL-1.1 |
| 나눔바른고딕 | `fonts/nanum-barun-gothic/` | 고딕 | 2 | Regular, Bold | OFL-1.1 |
| 나눔바른펜 | `fonts/nanum-barun-pen/` | 손글씨 | 2 | Regular, Bold | OFL-1.1 |
| 마루부리 | `fonts/maruburi/` | 명조 | 3 | Regular, SemiBold, Bold | OFL-1.1 |
| 나눔손글씨 아빠의 연애편지 | `fonts/nanum-hw-a-bba-eui-yeon-ae-pyeon-ji/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 암스테르담 | `fonts/nanum-hw-am-seu-te-reu-dam/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 바른히피 | `fonts/nanum-hw-ba-reun-hi-pi/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 부장님 눈치체 | `fonts/nanum-hw-bu-jang-nim-nun-ci-ce/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 철필글씨 | `fonts/nanum-hw-ceor-pir-geur-ssi/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 다행체 | `fonts/nanum-hw-da-haeng-ce/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 대한민국 열사체 | `fonts/nanum-hw-dae-han-min-gug-yeor-sa-ce/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 따악단단 | `fonts/nanum-hw-dda-ag-dan-dan/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 또박또박 | `fonts/nanum-hw-ddo-bag-ddo-bag/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 강부장님체 | `fonts/nanum-hw-gang-bu-jang-nim-ce/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 갈맷글 | `fonts/nanum-hw-gar-maes-geur/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 꽃내음 | `fonts/nanum-hw-ggoc-nae-eum/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 고딕 아니고 고딩 | `fonts/nanum-hw-go-dig-a-ni-go-go-ding/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 중학생 | `fonts/nanum-hw-jung-hag-saeng/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 마고체 | `fonts/nanum-hw-ma-go-ce/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 미니 손글씨 | `fonts/nanum-hw-mi-ni-son-geur-ssi/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 세계적인 한글 | `fonts/nanum-hw-se-gye-jeog-in-han-geur/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 나눔손글씨 야근하는 김주임 | `fonts/nanum-hw-ya-geun-ha-neun-gim-ju-im/` | 손글씨 | 1 | Regular | OFL-1.1 |
| G마켓 산스 | `fonts/gmarket-sans/` | 고딕 | 2 | Medium, Bold | OFL-1.1 |
| 에스코어 드림 | `fonts/s-core-dream/` | 고딕 | 6 | 4 Regular, 5 Medium, 6 Bold, 7 ExtraBold, 8 Heavy, 9 Black | 에스코어 글꼴 라이선스 |
| 페이퍼로지 | `fonts/paperlogy/` | 고딕 | 6 | 4 Regular, 5 Medium, 6 SemiBold, 7 Bold, 8 ExtraBold, 9 Black | OFL-1.1 |
| 프리젠테이션 | `fonts/freesentation/` | 고딕 | 6 | 4 Regular, 5 Medium, 6 SemiBold, 7 Bold, 8 ExtraBold, 9 Black | OFL-1.1 |
| 배달의민족 한나는 열한살 | `fonts/bm-hanna-11yrs/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 한나체 Air | `fonts/bm-hanna-air/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 한나체 Pro | `fonts/bm-hanna-pro/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 기랑해랑체 | `fonts/bm-kiranghaerang/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 을지로체 | `fonts/bm-euljiro/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 을지로10년후체 | `fonts/bm-euljiro-10yrs/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 을지로 오래오래체 | `fonts/bm-euljiro-oraeorae/` | 디자인 | 1 | Regular | OFL-1.1 |
| 배달의민족 꾸불림체 | `fonts/bm-kkubulim/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 카페24 PRO Slim Max | `fonts/cafe24-pro-slim-max/` | 고딕 | 1 | Max | OFL-1.1 |
| 카페24 PRO Slim Fit | `fonts/cafe24-pro-slim-fit/` | 고딕 | 1 | Fit | OFL-1.1 |
| 카페24 PRO Slim Air | `fonts/cafe24-pro-slim-air/` | 고딕 | 1 | Air | OFL-1.1 |
| 카페24 PRO UP | `fonts/cafe24-proup/` | 고딕 | 1 | Regular | OFL-1.1 |
| 카페24 모야모야 Face | `fonts/cafe24-moyamoya-face/` | 디자인 | 1 | Face | OFL-1.1 |
| 카페24 모야모야 | `fonts/cafe24-moyamoya/` | 디자인 | 1 | Regular | OFL-1.1 |
| 카페24 슈퍼매직 Bold | `fonts/cafe24-supermagic-bold/` | 디자인 | 1 | Bold | OFL-1.1 |
| 카페24 슈퍼매직 Regular | `fonts/cafe24-supermagic-regular/` | 디자인 | 1 | Regular | OFL-1.1 |
| 카페24 클래식타입 | `fonts/cafe24-classictype/` | 명조 | 1 | Regular | OFL-1.1 |
| 카페24 써라운드 에어 | `fonts/cafe24-ssurround-air/` | 디자인 | 1 | Light | OFL-1.1 |
| 카페24 써라운드 | `fonts/cafe24-ssurround/` | 디자인 | 1 | Bold | OFL-1.1 |
| 카페24 아네모네 에어 | `fonts/cafe24-ohsquare-air/` | 디자인 | 1 | Light | OFL-1.1 |
| 카페24 아네모네 | `fonts/cafe24-ohsquare/` | 디자인 | 1 | Regular | OFL-1.1 |
| 카페24 빛나는별 | `fonts/cafe24-shiningstar/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 카페24 고운밤 | `fonts/cafe24-oneprettynight/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 카페24 당당해 | `fonts/cafe24-dangdanghae/` | 디자인 | 1 | Regular | OFL-1.1 |
| 카페24 단정해 | `fonts/cafe24-danjunghae/` | 고딕 | 1 | Regular | OFL-1.1 |
| 카페24 심플해 | `fonts/cafe24-simplehae/` | 고딕 | 1 | Regular | OFL-1.1 |
| 카페24 동동 | `fonts/cafe24-dongdong-regular/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 카페24 쑥쑥 | `fonts/cafe24-ssukssuk-regular/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 카페24 숑숑 | `fonts/cafe24-syongsyong/` | 손글씨 | 1 | Regular | OFL-1.1 |
| 학교안심 우주 | `fonts/hakgyoansim-wooju/` | 디자인 | 1 | R | OFL-1.1 |
| 학교안심 가을소풍 | `fonts/hakgyoansim-gaeulsopung/` | 손글씨 | 1 | B | OFL-1.1 |
| 학교안심 분필 | `fonts/hakgyoansim-bunpil/` | 손글씨 | 1 | R | OFL-1.1 |
| 학교안심 지우개 | `fonts/hakgyoansim-jiugae/` | 디자인 | 1 | R | OFL-1.1 |
| 학교안심 몽글몽글 | `fonts/hakgyoansim-monggeulmonggeul/` | 디자인 | 1 | R | OFL-1.1 |
| 학교안심 물결 | `fonts/hakgyoansim-mulgyeol/` | 디자인 | 2 | R, B | OFL-1.1 |
| 학교안심 봄방학 | `fonts/hakgyoansim-bombanghak/` | 디자인 | 1 | R | OFL-1.1 |
| 학교안심 바른바탕 | `fonts/hakgyoansim-bareonbatang/` | 명조 | 2 | R, B | OFL-1.1 |
| 학교안심 바른돋움 | `fonts/hakgyoansim-bareondotum/` | 고딕 | 2 | R, B | OFL-1.1 |
| 학교안심 꾸러기 | `fonts/hakgyoansim-ggooreogi/` | 디자인 | 1 | R | OFL-1.1 |
| 학교안심 산뜻돋움 | `fonts/hakgyoansim-santteutdotum/` | 고딕 | 1 | M | OFL-1.1 |
| 학교안심 둥근미소 | `fonts/hakgyoansim-dunggeunmiso/` | 디자인 | 2 | R, B | OFL-1.1 |

## 넣지 않은 글꼴과 까닭

| 글꼴 | 까닭 |
|---|---|
| 여기어때 잘난체 | 약관 표에서 「임베딩(앱·서버 안 글꼴 탑재)」이 △(조건부)이고 홀로 다시 배포하는 경우가 분명하지 않음 |
| tvN 즐거운이야기 | 약관에 「다른 소프트웨어와 묶어 재배포할 때 출처 표기」만 있고, 홀로 다시 배포·상업 사용이 분명히 적혀 있지 않음 |
| 티몬 몬소리체 | 공식 배포처(티몬)가 문을 닫아 약관 원문과 공식 파일을 확인할 수 없음 |
| 샌드박스 어그로체 | 공식 페이지(sandbox.co.kr/font)가 열리지 않고(404), 남은 안내 글이 「재배포 금지」와 「재배포 가능」으로 엇갈림 |
| 넥슨 Lv.1 고딕·메이플스토리 | 공식 배포처(levelup.nexon.com)에 접속되지 않아 약관 원문을 확인할 수 없음 |
| 학교안심 외 교육저작권지원센터의 다른 회사 글꼴 | 센터가 「KERIS 공모폰트를 제외한 폰트는 제작사 규정이 다를 수 있다」고 적어 둠 — KERIS 가 저작권자인 것만 넣음 |
| 배달의민족 글림체 | 글꼴 파일이 아니라 그림(PNG) 묶음 |
| 배달의민족 주아·도현·연성, 나눔손글씨 펜·붓 | 앱이 다른 길(구글 폰트)로 이미 받음 |
| 나눔스퀘어_ac | 한글이 일부만 들어 있는 판(같은 모양의 전체 판을 넣음) |
| 가는 굵기(Thin·ExtraLight·Light 등) | 자막에 잘 안 쓰여 뺌(써라운드·아네모네 Air 처럼 굵기가 아니라 다른 글꼴인 것은 넣음) |

## 내려 달라는 요청

글꼴 저작권자이신데 이 저장소에서 내려 주기를 바라시면 연락 주세요.

- 연락처: (대표 확인 — 아직 비어 있음)
