# EasyDoMix

인터넷 권한 없는 안드로이드 영상 · 오디오 편집 앱. 여러 영상 트랙 + 여러 오디오 트랙 타임라인, 트랙별 소리 조절, 자막, mp4 · m4a · wav 내보내기. EasyDo 시리즈.

## 다운로드

최신 버전 0.2.0 — [Releases](https://github.com/parkrye/AppProject_EasyDoMix/releases)에서 `EasyDoMix-<버전>.apk`를 받아 설치. Android 8.0 이상.

- 처음 설치 시 "출처를 알 수 없는 앱" 설치 허용 필요. Play 프로텍트가 검사 화면을 띄울 수 있음
- 업데이트는 새 APK를 같은 방식으로 덮어 설치. 프로젝트 · 설정 유지
- 앱 안 업데이트 알림 없음. `설정 → 앱 정보 → 새 버전 받기`로 Releases 페이지 열기
- 서명 인증서 SHA-256: `c4068225381b81f1cc4d102bf7f6e5a601750506eb85f201520126b60ab96851`
  (`apksigner verify --print-certs EasyDoMix-<버전>.apk`로 확인)

## 기능

- 프로젝트: 화면 비율(16:9 · 9:16 · 1:1), 이름 변경 · 복제 · 삭제, 자동 저장
- 타임라인: 영상 트랙(위가 앞 레이어) · 오디오 트랙 여러 개, 자막 트랙. 재생 위치 가운데 고정, 가로로 끌어 이동, 두 손가락 확대 · 축소
- 클립: 사진 선택기 · 파일로 영상 · 오디오 · 이미지 추가, 끌어 옮기기(위아래 같은 종류 트랙으로도), 양 끝 핸들로 길이 자르기, 재생 위치에서 나누기, 삭제, 복제, 맞춰 붙이기(클립 끝 · 재생 위치 · 자막 경계에 자석처럼 붙음), 실행 취소 · 다시 실행
- 소리 조절: 트랙 소리 크기 · 좌우 위치 · 음소거 · 단독 재생, 클립 소리 크기 · 좌우 위치 · 음소거 · 페이드 인/아웃, 구간별 볼륨(재생 위치마다 소리 크기를 정하면 사이는 자연스럽게 이어짐), 음색(저음 · 중음 · 고음 3단), 소리 크기 맞추기(가장 큰 소리가 찢어지지 않을 만큼), 음 높이(반음 -12~+12), 전체 소리 크기, 트랙 · 전체 소리 크기 표시(재생 시각에 맞춤), 영상 속 소리 분리(오디오 트랙에 새 클립)
- 빠르기: 영상 0.25~4배, 오디오 파일 0.5~2배. 빠르기를 바꿔도 음 높이 유지
- 영상: 위 트랙을 작은 창(화면 속 화면)으로 겹치기(위치 · 크기 · 투명도, 미리 정한 배치), 앞 클립과 겹쳐 넘어가기 · 디졸브 전환, 밝기 · 대비 · 채도
- 화면 용어: 쉬운 말(클립 설정 · 소리 조절 · 맞춰 붙이기 · 음소거 · 단독 재생 · 좌우 위치), 버튼 길게 누르기 설명, 편집 화면 ? 용어 모음
- 자막: 텍스트 · 시작/끝 · 위치 · 크기 · 글자색 · 외곽선 색 · 두께, SRT 가져오기 · 내보내기, 내보낼 때 영상에 입히기 선택
- 내보내기: mp4(H.264 · AAC, 480p · 720p · 1080p, 영상 화질 3단계, 오디오 128~320kbps), 오디오만 m4a(AAC) · wav(16비트 PCM). 진행률 · 취소, 알림에 진행률 표시
- 설정: 화면(배경화면 색 사용, 기본 꺼짐) · 데이터(백업 만들기 · 백업에서 복원) · 앱 정보(앱 정보 · 새 버전 받기 · 오픈소스 라이선스)

원본 미디어는 앱으로 복사하지 않고 선택한 파일을 그대로 참조합니다. 원본을 옮기거나 지우면 프로젝트에서 열 수 없습니다.

알려진 제한

- 미리보기는 기기 성능에 맞춰 낮은 해상도로 합성합니다. 영상 여러 개가 동시에 나오는 구간(전환 · 화면 속 화면)은 기기에 따라 미리보기가 끊길 수 있습니다
- 백업에는 미디어 원본이 들어가지 않습니다

버그 · 제안은 [Issues](https://github.com/parkrye/AppProject_EasyDoMix/issues)에.

## 개인정보

- 인터넷 권한 없음 · 광고 없음 · 수집 · 전송 없음. 계정 · 사용 통계 · 오류 보고 없음
- 프로젝트는 기기 안에만 저장. 앱 삭제 시 함께 삭제
- 앱 안 백업 · 복원(파일 하나, `easydomix-backup-yyyy-MM-dd.json`): 프로젝트 · 설정 포함, 미디어 원본은 미포함 — 다른 기기에서 복원하면 원본 파일을 다시 연결할 수 없음
- 내보낸 영상 · 오디오 · 자막 · 백업 파일은 사용자가 고른 위치에만 저장

## EasyDo 시리즈

| 앱 | 용도 | 플랫폼 |
|---|---|---|
| [EasyDoDraw](https://github.com/parkrye/MultiProject_EasyDoDraw) | 그림 · 애니메이션 | Android · Windows |
| [EasyDoWrite](https://github.com/parkrye/AppProject_EasyDoWrite) | 소설 · 글쓰기 | Android |
| [EasyDoRead](https://github.com/parkrye/AppProject_EasyDoRead) | 책 · 문서 읽기 | Android |
| [EasyDoShelve](https://github.com/parkrye/AppProject_EasyDoShelve) | 웹 소설 서재 | Android |
| [EasyDoPhoto](https://github.com/parkrye/AppProject_EasyDoPhoto) | 카메라 · 사진 편집 | Android |
| [EasyDoDiet](https://github.com/parkrye/AppProject_EasyDoDiet) | 식단 · 운동 기록 | Android |
| [EasyDoZip](https://github.com/parkrye/AppProject_EasyDoZip) | 파일 · 압축 관리 | Android |
| [EasyDoGame](https://github.com/parkrye/AppProject_EasyDoGame) | 미니 게임 모음 | Android |
| [EasyDoMix](https://github.com/parkrye/AppProject_EasyDoMix) | 영상 · 오디오 편집 | Android |
| [EasyDoRecord](https://github.com/parkrye/AppProject_EasyDoRecord) | 녹음 | Android |
| [EasyDoStudio](https://github.com/parkrye/DesktopProject_EasyDoStudio) | 화면 녹화 · 영상 편집 | Windows |

## 라이선스

MIT License · © parkrye. 포함된 서드파티 라이브러리 고지는 앱 안 `설정 → 앱 정보 → 오픈소스 라이선스`에서 확인. FFmpeg 등 GPL 계열 라이브러리 없음.
