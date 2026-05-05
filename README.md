# JHK FENCING CLUB 홈페이지 사용 가이드

## 📁 포함된 파일

```
jhk-fencing-club.html    # 홈페이지 본체 (HTML 단일 파일)
jhk-logo.jpg             # 클럽 로고
coach-jhk.jpg            # 장현경 대표감독 프로필 사진
README.md                # 이 가이드 문서
```

---

## 🚀 1단계: 호스팅 (홈페이지 인터넷 공개)

세 파일을 **같은 폴더**에 넣고 다음 중 한 곳에 업로드하시면 됩니다.

### 추천 무료 호스팅 (가장 쉬움)
- **Netlify Drop** (https://app.netlify.com/drop)
  - 폴더 통째로 끌어다 놓으면 끝. 1분 안에 URL 발급
  - 예: `https://jhk-fencing.netlify.app`
  - 무료, 광고 없음, HTTPS 자동 적용

- **Vercel** (https://vercel.com)
  - Netlify와 비슷, 더 빠른 속도

- **Cloudflare Pages** (https://pages.cloudflare.com)
  - 한국에서 가장 빠른 속도

### 도메인 연결 (선택사항)
- 가비아, 후이즈에서 도메인 구매 (예: `jhkfencing.com`)
- Netlify/Vercel 설정에서 도메인 연결 (5분 작업)

---

## ⚙️ 2단계: 형님이 직접 수정하실 곳

HTML 파일을 메모장 또는 VS Code로 열어서 수정하시면 됩니다.

### 1. 카카오톡 채널 URL
HTML 파일에서 `https://pf.kakao.com/` 검색 → 형님 채널 URL로 변경

### 2. 네이버톡톡 URL
`https://talk.naver.com/` 검색 → 형님 톡톡 URL로 변경

### 3. SNS 링크
- `https://instagram.com` → 클럽 인스타그램 URL
- `https://youtube.com` → 클럽 유튜브 URL
- `https://tiktok.com` → 클럽 틱톡 URL

### 4. 관리자 비밀번호
HTML 파일에서 `const ADMIN_PW='jhk2026'` 검색 → 원하는 비밀번호로 변경

### 5. 영상 파일 추가 (선택사항)
같은 폴더에 다음 파일을 추가하면 자동으로 배경 영상이 재생됩니다.
- `intro.mp4` — 인트로 5초 영상
- `hero-bg.mp4` — 히어로 섹션 배경 영상 (10~20초 루프)

영상이 없어도 페이지는 정상 작동합니다.

---

## 🎬 영상 추천 사양

- 해상도: **1920x1080** (가로) 또는 **1080x1920** (세로)
- 용량: **2~5MB 이하** (모바일 로딩 최적화)
- 코덱: **H.264 mp4**
- 영상 압축: https://www.freeconvert.com/video-compressor

---

## 📷 사진 교체

### 갤러리 사진 추가
HTML 파일에서 `<!-- GALLERY -->` 섹션을 찾아서 각 `<div class="gallery-item">` 안에 다음과 같이 이미지를 넣어주세요.

```html
<div class="gallery-item">
  <img src="gallery1.jpg" alt="훈련" style="width:100%;height:100%;object-fit:cover;">
  <span class="gallery-tag">— Training</span>
</div>
```

같은 폴더에 `gallery1.jpg`, `gallery2.jpg` ... 형식으로 사진 6장 정도 올려주시면 됩니다.

### 사진 압축 도구 (추천)
- https://tinypng.com — 드래그&드롭으로 자동 압축
- 모바일에서 빠르게 로딩되려면 **각 사진 200KB 이하** 권장

---

## 🔧 자주 묻는 수정사항

### 클럽 주소 상세하게 표시하고 싶을 때
HTML에서 `상세 주소는 문의 시 안내` 부분을 찾아서 실제 주소로 변경

### 운영 시간 변경
`평일 14:00 — 22:00` 부분을 검색해서 수정

### 슬로건 변경
`검의 길 위에서` 부분 검색해서 수정

### 코치 명언 변경
`펜싱은 칼이 아니라 마음으로 하는 운동입니다` 부분 검색해서 수정

---

## 📊 관리자 페이지 사용법

1. 페이지 하단까지 스크롤
2. 푸터 맨 아래 작은 `· admin ·` 링크 클릭
3. 비밀번호 입력 (기본값: `jhk2026`, 변경 권장)
4. 로그인 후 모든 문의 내역 확인 가능

문의는 자동으로 브라우저에 저장되며, 관리자 페이지에서 이름·연락처·내용·시간을 모두 확인할 수 있습니다.

---

## 💡 추가 기능 추천 (필요시 요청)

- 수강료 안내 섹션
- FAQ (자주 묻는 질문) 섹션
- 블로그 / 클럽 소식 섹션
- 회원 후기 / 리뷰 섹션
- 카카오맵 / 네이버지도 실제 임베드
- 다국어 지원 (영문)

추가로 필요한 기능 있으시면 언제든 말씀해주세요.

---

**JHK FENCING CLUB · 장현경펜싱클럽**
Honor & Discipline
