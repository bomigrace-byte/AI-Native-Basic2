# 🎬 미션 2. 멀티모달 AI 브랜드 광고 제작

> 텍스트로 이미지 한 장 만드는 건 누구나 합니다.
> 이번엔 **기획 의도 → 프롬프트 → 결과물 → 통합 편집**으로 이어지는
> **제작 파이프라인 전체를 스스로 설계**하고, **10초 이내 브랜드 광고 영상**을 완성합니다.

---

## 📦 최종 제출물 (3가지)

| # | 산출물 | 형식 | 비고 |
|---|--------|------|------|
| ① | **스토리보드(기획 문서)** | PDF 1개 | 씬별 필수 필드 포함 |
| ② | **광고 영상** | MP4 1개 | 10초 이내 |
| ③ | **이 README** | md | 진행 체크·의사결정 기록 |

> ✂️ **핵심은 "도구를 많이 쓰는 것"이 아니라, 왜 그렇게 결정했는지 설명하는 것입니다.**

---

## STEP 0. 브랜드 & 캠페인 정의

가상 또는 실제 브랜드 **1개**를 선정합니다.

```
- 브랜드명: SEREN

https://github.com/user-attachments/assets/469d3094-468b-4207-b28b-662a207b41c6


- 타겟: 20~30대 번아웃 직장인
- 톤앤매너: 미니멀, 자연친화적, 시네마틱, 따뜻한 고요함
- USP(차별점): "일상의 틈새에서 찾는 단 한 번의 호흡" — 복잡한 세상 속 가장 쉬운 회복 루틴
- 광고 목적: 브랜드 인지
- 핵심 메시지(한 문장): "잠깐, 숨 한번 고르고 가요."
```

> ✂️ **판정 기준** → 타겟·톤앤매너·USP 3개가 모두 채워졌는가? 메시지가 **한 문장**인가?

---

## STEP 1. 사용 도구 확정 + 대체 도구 준비

**이미지 / 비디오 / 오디오 각 1종 이상** 필수. 그리고 막힐 때를 대비해 **대체 도구도 각 1개**.

| 역할 | 메인 도구 | 선택 이유 | 대체 도구(대비용) |
|------|-----------|-----------|-------------------|
| 이미지 생성 | DALL-E 3 | 비용 우선 고려(무료), 초보자 최적 | Gemini(대화형 AI이므로 품질이 떨어질 수 있음) |
| 비디오 생성/변환 | Pollo AI | 비용 우선 고려(무료), 초보자 최적 | Hailuo AI(초반에 지급해주는 크레딧 외에는 유료 결제해야함) |
| 오디오 생성 | Eleven Labs | 비용 우선 고려(무료), 내레이션에 최적 | Clova AI | (목소리 스타일이 많이 없음)
| BGM 생성 | Suno AI | 무료, AI 음악 최강자 | Udio | (인터페이스가 복잡하고, 사용하기 어려움)

> ✂️ **판정 기준** → 이미지·비디오·오디오 3종이 모두 있는가? 대체 도구가 각 1개씩 있는가?
> 💡 대기열/플랜 제한으로 막힐 수 있으니 **도구명만이라도** 미리 적어두세요.

---

## STEP 2. 스토리보드 작성 (→ 별도 PDF)

씬 단위로 나누고, **모든 씬 공통 8개 필드**를 누락 없이 채웁니다.

```
## 씬 [1]
- 씬 길이(초): 2
- 목표 메시지: 오늘도 지친 직장인의 모습
- 화면 구성: 창가에 앉은 직장인 실루엣/ 책상 위 노트북 화면 빛만 보임/ 표정은 보이지 않고 어깨가 축 처진 뒷모습/ 텍스트 없음
- 내레이션/카피: "오늘도 지쳤나요?"
- 사용 도구 및 목적:
   - 이미지 생성 : Dall-E3 (키 비주얼 생성)
   - 비디오 생성 : Pollo AI (이미지를 짧은 영상으로 변환)
   - 오디오 생성 : Eleven Labs (내레이션) + Pixabay (Sound Effects - City ambient night)
   - 편집 : Capcut - 영상에 오디오 레이어 배치
- 입력 프롬프트(원문): 
A tired office worker sitting alone by a large window at dusk,
seen from behind as a silhouette,
slouched shoulders, dim laptop glow on the desk,
city skyline outside the window in deep blue dusk light,
stacked papers and a cold coffee cup on the desk,
cinematic film photography style,
desaturated cool blue and grey tones,
dim and fading light, no golden sunset,
35mm film grain texture, soft vignette,
heavy and melancholic atmosphere,
no face visible,
★cinematic widescreen format 16:9 aspect ratio,
★wide establishing shot,
★horizontal composition optimized for 16:9 frame,
★letterbox cinematic framing
- 출력 결과 요약: "도심 야경을 배경으로 홀로 노트북 앞에 앉은 실루엣, 쌓인 서류와 커피잔이 말해주는 고독한 야근의 순간"
- 결과 파일명/링크: Scene01_keyvisual.png/ Scene01(Pollo)_motion.mp4/ Scene01_narration(Eleven Labs).mp3/ Scene01_soundeffect-cityabientnight(Pixabay).mp3
https://github.com/user-attachments/assets/b1031fc1-e895-4ea5-b863-4c140074bb42
```

```
## 씬 [2]
- 씬 길이(초): 3
- 목표 메시지: SEREN 앱으로 분위기 전환
- 화면 구성: 스마트폰 화면에 SEREN 앱이 빛나는 장면 / 손이 스마트폰 화면을 탭 / 화면에서 딥 티얼 + 그린세이지 빛이 번지듯 퍼져나옴 / 텍스트 없음
- 내레이션/카피: "숨을 들이쉬어 보세요."
- 사용 도구 및 목적:
   - 이미지 생성 : Dall-E3 (키 비주얼 생성)
   - 비디오 생성 : Pollo AI (이미지를 짧은 영상으로 변환)
   - 오디오 생성 : Eleven Labs(내레이션) + Pixabay(Sound Effects - Bird chipping, soft wind)
   - 편집 : Capcut - 영상에 오디오 레이어 배치
- 입력 프롬프트(원문):
Close-up of two hands gently holding a smartphone,
phone screen facing LEFT side of frame, hands angled toward left,
SEREN meditation app displayed on screen,

★ app UI background shows a serene nature scene inside the screen,
★ misty forest with tall pine trees reflected on still water,
★ calm lake surface with gentle ripples surrounding the breathing circle,
★ trees and water reflection visible around the glowing circle,
★ soft fog and mist between the trees on screen background,

app UI featuring deep teal and sage green tones,
soft glowing breathing circle in the center of screen,
glowing white-teal breathing circle with "Breathe In" text and countdown timer,
gentle gradient from deep ocean teal to soft forest sage,
nature scene of still water and misty pine forest as app background,
bottom navigation bar with Sleep, Focus, Breathe icons,
SEREN logo and tagline visible at top of screen,

★ screen brightness is ENHANCED and MORE LUMINOUS than ambient light,
★ phone screen emits a visible soft teal-green glow onto hands,
★ teal-green screen light softly reflects and spills onto fingers and palms,
★ subtle teal light cast visible on skin texture of hands,
★ screen is the brightest element in the scene,

soft teal-green light from screen illuminating hands clearly,
hands are well-lit by the phone screen glow,
background is softly blurred dark room,
warm dim candlelight in background,
cinematic photography style,
shallow depth of field,
calm, healing, grounded atmosphere,
no purple, no lavender, no bright neon colors,
35mm film grain, gentle vignette,
natural and organic color palette,
screen brightness is the main light source,
crisp UI details visible on screen,

★ cinematic widescreen format 16:9 aspect ratio,
★ horizontal composition optimized for 16:9 frame,
★ letterbox cinematic framing

- 출력 결과 요약: "촛불이 켜진 어두운 공간에서 명상 앱 화면의 청록빛을 두 손으로 감싸 쥔 채, 숨 고르기 하나에 온전히 집중하는 고요한 위로의 순간"
- 결과 파일명/링크: Scene02_keyvisual.png/ Scene02(Pollo)_motion.mp4/ Scene02_narration(Eleven Labs).mp3/ Scene02,03,04_soundeffect-birdchipping(Pixabay).mp3/ Scene02,03,04_soundeffect-soft wind(Pixabay).mp3
https://github.com/user-attachments/assets/0c486d93-a157-4c63-a10d-a3c150d49169
```

```
## 씬 [3]
- 씬 길이(초): 3
- 목표 메시지: SEREN 앱으로 치유되는 과정
- 화면 구성: 햇살이 비치는 분위기로 눈을 감은 얼굴 클로즈업 / 표정이 서서히 부드럽게 풀림 /  배경 — 딥 티얼 빛 보케 / 창문 너머 나뭇잎 흔들림 / 텍스트 없음
- 내레이션/카피: "나로 돌아오세요."
- 사용 도구 및 목적:
   - 이미지 생성 : Dall-E3 (키 비주얼 생성)
   - 비디오 생성 : Hailuo AI (이미지를 짧은 영상으로 변환)
   - 오디오 생성 : Eleven Labs (내레이션) + Suno AI (BGM)
   - 편집 : Capcut - 영상에 오디오 레이어 배치
- 입력 프롬프트(원문):
Close-up of two hands gently holding a smartphone,
phone screen facing LEFT side of frame, hands angled toward left,
SEREN meditation app displayed on screen,

★ app UI background shows a serene nature scene inside the screen,
★ misty forest with tall pine trees reflected on still water,
★ calm lake surface with gentle ripples surrounding the breathing circle,
★ trees and water reflection visible around the glowing circle,
★ soft fog and mist between the trees on screen background,

app UI featuring deep teal and sage green tones,
soft glowing breathing circle in the center of screen,
glowing white-teal breathing circle with "Breathe In" text and countdown timer,
gentle gradient from deep ocean teal to soft forest sage,
nature scene of still water and misty pine forest as app background,
bottom navigation bar with Sleep, Focus, Breathe icons,
SEREN logo and tagline visible at top of screen,

★ screen brightness is ENHANCED and MORE LUMINOUS than ambient light,
★ phone screen emits a visible soft teal-green glow onto hands,
★ teal-green screen light softly reflects and spills onto fingers and palms,
★ subtle teal light cast visible on skin texture of hands,
★ screen is the brightest element in the scene,

soft teal-green light from screen illuminating hands clearly,
hands are well-lit by the phone screen glow,
background is softly blurred dark room,
warm dim candlelight in background,
cinematic photography style,
shallow depth of field,
calm, healing, grounded atmosphere,
no purple, no lavender, no bright neon colors,
35mm film grain, gentle vignette,
natural and organic color palette,
screen brightness is the main light source,
crisp UI details visible on screen,

★ cinematic widescreen format 16:9 aspect ratio,
★ horizontal composition optimized for 16:9 frame,
★ letterbox cinematic framing

- 출력 결과 요약: "눈을 감은 채 햇살을 온몸으로 받아들이는 미소, 초록빛 보케와 황금빛 빛 입자 속에서 피어나는 평온한 해방감"
- 결과 파일명/링크: Scene03_keyvisual.png/ Scene03(Hailuo)_motion.mp4/ Scene03_narration(Eleven Labs).mp3/ Scene03,04_bgm-Piano(Suno).mp3/ Scene02,03,04_soundeffect-birdchipping(Pixabay).mp3/ Scene02,03,04_soundeffect-soft wind(Pixabay).mp3
https://github.com/user-attachments/assets/8894f26c-a04f-473a-acf2-385362a8b59b
```

```
## 씬 [4]
- 씬 길이(초): 2
- 목표 메시지: SEREN 앱 인지 + 접속 유도
- 화면 구성: 중앙에 SEREN 로고 / 로고 주변 신비로운 Circle / 로고 아래 슬로건 텍스트 등장
- 내레이션/카피: 없음 (여운을 위한 침묵) / ① SEREN (브랜드명) / ② "Breathe in. Come back to yourself." (슬로건) / ③ "잠깐, 숨 한번 고르고 가요. →" (CTA)
- 사용 도구 및 목적:
   - 이미지 생성 : Gemini (키 비주얼 생성)
   - 비디오 생성 : Google Flow (이미지를 짧은 영상으로 변환)
   - 편집 : Capcut - 영상에 오디오 레이어 배치
- 입력 프롬프트(원문):
A delicate and soft-featured Korean woman in her mid 20s,
slender fine facial features, soft jawline, gentle face,
porcelain-like smooth skin with natural warmth,
eyes gently closed with long soft lashes,
subtle peaceful smile, lips softly curved upward,
expression of pure tranquility and quiet bliss,
youthful and ethereal beauty,
hair softly flowing down, loose and natural,

SOFT warm golden sunlight gently touching her face,
NOT overexposed, NOT blown out,
sunlight is gentle and diffused, NOT harsh or intense,
face evenly and softly lit with warm golden glow,
delicate sun rays softly landing on cheeks and forehead,
skin luminous, translucent and porcelain-like under soft light,

subtle golden bokeh sparkles in the air,
magical light shimmer effect around her,
soft glowing halo of light around her silhouette,
dreamy sparkling atmosphere like morning dew catching light,
ethereal light flares softly dancing near her face,

background bokeh EXACTLY 50% warm golden yellow
AND 50% soft sage green,
sage green bokeh circles clearly visible
on the RIGHT side of background,
golden bokeh on LEFT side near window,
lush green nature visible through window,
background bright and airy,

overall mood soft, healing, luminous and magical,
feeling of gentle morning light and inner renewal,

shallow depth of field,
wearing soft cream or white top,
cinematic film photography style,
healing and renewal mood,
ultra realistic, 8K,

★ cinematic widescreen format 16:9 aspect ratio,
★ horizontal composition optimized for 16:9 frame,
★ letterbox cinematic framing,
★ subject positioned slightly left of center,
★ bokeh background fills wide horizontal frame naturally

- 출력 결과 요약: "깊은 심해빛 어둠 속에서 은은하게 빛나는 원형 오라와 함께, 'SEREN'이라는 이름이 조용히 당신을 자신에게로 되돌려 보내는 초대"
- 결과 파일명/링크: Scene04_keyvisual.png/ Scene04(Google Flow)_motion.mp4/ Scene03,04_bgm-Piano(Suno).mp3/ Scene02,03,04_soundeffect-birdchipping(Pixabay).mp3/ Scene02,03,04_soundeffect-soft wind(Pixabay).mp3
https://github.com/user-attachments/assets/e4d8bbd4-496a-4114-a681-7588f4889a8d
```


> ✂️ **판정 기준** → 모든 씬이 **8개 필드**를 다 채웠는가? 파일명 규칙이 **일관**적인가?

---

## STEP 3. 프롬프트 개선 로그 (최소 1개 씬 필수)

"운 좋게 나온 결과"가 아니라 **의도적으로 개선했다**는 증거입니다.

```
## 씬 [1] 프롬프트 개선 로그
- 수정 전 의도 : “어두운 사무실 안 책상에 앉은 직장인의 뒷모습”
- 문제 : 노을 지는 풍경의 외부 분위기로 어두운 무드가 부족
- 수정 후 변경 : “창밖의 하늘은 딥 블루 색상, 빛은 사라지고, 노을 삭제”로 프롬프트 조정
- 결과 변화 : 빛이 없는 어두운 사무실 풍경으로 반영됨.
```
```
## 씬 [2] 프롬프트 개선 로그
- 수정 전 의도 : “캔들하나가 밝혀진 어두운 실내에 어플에서 흘러나오는 청록빛 색감이 손을 감싸며 자연 속 고요함을 손안에서 발견”
- 문제 : 밝기가 너무 어두워서 발견의 느낌이 부족, 어플 화면이 바뀜
- 수정 후 변경 : “밝기 조절, 스마트폰 화면은 숲 + 호수, 원 주변에 나무와 물 반영이 보이게” 프롬프트 조정
- 결과 변화 : 전체적으로 청록빛 색감으로 은은히 빛나는 자연 풍경 화면 반영됨.
```
```
## 씬 [3] 프롬프트 개선 로그
- 수정 전 의도 : “어플을 통해 치유되며 온화하게 변하는 여성의 얼굴”
- 문제 : 여성의 캐릭터(나이, 머리스타일) 바뀜, 치유되는+몽환적 느낌 부족,
- 수정 후 변경 : “캐릭터 얼굴 묘사 상세히, 치유 색상, 햇살 강도, 빛 효과 명시” 프롬프트 조정
- 결과 변화 : 자연 색감으로 치유 느낌을 극대화 하며 부드러운 미소를 머금은 여성 반영.
```
```
## 씬 [4] 프롬프트 개선 로그
- 수정 전 의도 : “부드러운 골드색상으로 로고 노출”
- 문제 : 골드 색상이 이전 씬의 색상과 불일치, 생동감 있는 로고 표현 필요
- 수정 후 변경 : “로고 색상 골드 → 티얼 화이트, 로고 주변 원형 이펙트 추가” 프롬프트 조정
- 결과 변화 : 정체성에 맞는 일관성있는 색상 반영, 로고의 에너지 극대화
```

> ✂️ **판정 기준** → **무엇을 / 왜 / 어떤 결과로** 바꿨는지 3가지가 다 있는가?

---

## STEP 4. 일관성(캐릭터/스타일) 유지 전략 (권장)

멀티모달의 최대 난관 = **캐릭터·화풍 불일치**. 미리 고정하세요.

```
- 사용한 일관성 기능: cref, sref의 경우 Midjourney의 기능이므로 해당 없음, ControlNet은 Stable Diffusion의 기능이므로 해당 없음
- 고정한 파라미터/레퍼런스: 딥티얼 + 그린세이지 색감 및 분위기 고정/프롬프트마다 명시하였음
- 고정한 이유: 브랜드의 정체성을 나타내는 색감이라 고정하였음
```

> ✂️ **판정 기준** → "어떤 레퍼런스/파라미터를 고정했는지" 발표에서 설명할 수 있는가?

---

## STEP 5. 크레딧 부족 대응 전략 (택 1 이상)

영상 생성은 크레딧 소모가 큽니다. **이미지 단계에서 스토리보드를 확정한 뒤** 영상 변환하세요.

- [✔️] 씬 수 줄이고 메시지 밀도 높이기 : 10초 기준 4씬
	*씬축소를 위한 유지씬 : 각 씬의 키비주얼 및 핵심 메시지 선정하여 유지
- [✔️] 정지 이미지 + 짧은 모션(패닝/줌/루프) 중심 구성
	*T2I와 I2V의 차이점 및 선택 기준
	-Text to Image : 텍스트 설명으로 원하는 이미지를 생성
	- Image to Video : 레퍼런스 이미지로 원하는 영상을 생성
	- 선택 기준 : 아무런 레퍼런스가 없을 경우 T2I, 키비주얼 이미지가 있을 경우 정교한 영상제작을 위해 I2V 
- [✔️] 동일 스타일 레퍼런스 고정으로 재생성 횟수 줄이기: 재생성 횟수 씬당 이미지 5회, 영상 3회 이하

> ✂️ **판정 기준** → 위 3개 중 **최소 1개** 전략을 선택·적용했는가?

---

## STEP 6. 통합 편집 (편집 도구는 "보조"만!)

```
- 사용 편집 도구: CapCut
- 편집 범위: 컷 편집, 오디오 레이어
```

> ✂️ **⚠️ 제약** → 편집 도구는 **통합 편집 용도만**. 핵심 비주얼/오디오는
> 반드시 **AI 생성 결과물이 주된 소스**여야 합니다.

---

## STEP 7. 서사 & 브랜드 인지장치

```
- 스토리라인 구조: 기승전결
- 마지막 3~5초 인지장치: 로고 / 슬로건 / CTA
```

> ✂️ **판정 기준** → 단순 컷 나열이 아닌가? **마지막 3~5초**에 브랜드 장치가 있는가?

---

## STEP 8. 최종 영상 스펙 확인

```
- 파일명: SEREN.mp4
- 길이: 10초
- 해상도: 720p (권장 720p 이상) / 해상도,색감 불일치 시 : 1. 프롬프트에 색감, 해상도 명시 3. 같은 생성모델 이용
- 프레임레이트: 25fps
- 코덱: H.264 / AAC
```

> ✂️ **판정 기준** → **10초 이내**인가? 720p 이상인가? AI 시각+청각 요소가 모두 있는가?

---

## ✅ 최종 제출 전 셀프 체크리스트

**필수**
- [✔️] 브랜드 아이덴티티 (타겟/톤앤매너/USP) 정의
- [✔️] 핵심 메시지 한 문장
- [✔️] 모든 씬 8개 필드 완료 (PDF)
- [✔️] 프롬프트 수정 전/후 최소 1개
- [✔️] 이미지·비디오·오디오 AI 각 1종 + 선택 이유
- [✔️] 영상 10초 이내 + AI 시청각 포함
- [✔️] 서사 구조 + 마지막 3~5초 브랜드 장치
- [✔️] 크레딧 대응 전략 1개
- [✔️] 대체 도구 각 1개
- [✔️] 스토리보드 PDF + MP4 제출

**⛔ 금지 (감점/실격)**
- [ ] 직접 촬영·유료 스톡 소스 사용 ❌
- [ ] 딥페이크·유해 콘텐츠 ❌
- [ ] 편집 도구로 핵심 비주얼 제작 ❌

**🎁 보너스 (선택)**
- [✔️ ] 립싱크 적용 : 기존 영상앞에 "하, 지친다"라고 말하는 여자 모습이 담긴 씬 추가
  <img width="1672" height="941" alt="Scene00_ad_keyvisual" src="https://github.com/user-attachments/assets/ca976140-65a9-4027-ab81-22360b91a489" />
- [✔️ ] 동일 스토리보드, 다른 도구 재제작 : adobe firefly, google flow로 Scene02,04 재제작
  https://github.com/user-attachments/assets/d5ff7b11-2058-451f-9006-ee475f09fa65
  https://github.com/user-attachments/assets/ec99e188-fd30-4666-9946-6fefbc374005
- [✔️] 화면 비율 버전 2개 이상 : 16:9 / 9:16 / 1:1
  *파일 크기가 커서 github에 별도로 업로드하였습니다. 


