# 위클리 플래너 + 공부 타이머 (Weekly Planner + Study Timer)

한 파일(`index.html`)로 된 주간 시간표 + 공부 타이머. GoodNotes 플래너처럼 한 줄 = 1시간, 한 칸 = 10분 정사각형 격자.
A single-file weekly time-grid planner with a study timer. One row = 1 hour, one square = 10 minutes.

## 기능 / Features
- 10분 격자 시간표(드래그로 만들기·옮기기·늘이기, 지금 시간 자석, 3개 이상 겹치면 빨간 테두리)
- 반복 블록, 습관 트래커(주 단위), 할 일·목표, 다크 모드
- 공부 타이머: 과목별 스톱워치, 뽀모도로(원형 다이얼), 항상 위 팝업(PiP), 폰용 보조 화면
- 표시 시간 기본 6시 ~ 다음 날 새벽 3시 (설정에서 변경)

## 쓰는 법 / Usage
이 앱은 claude.ai Artifact(저장소 `db` 기능과 Notion 연결)로 돌아가도록 만들었습니다. 파일을 그냥 브라우저로 열면 "미리보기 모드"로 이 브라우저(localStorage)에만 저장됩니다.
It is built to run as a claude.ai Artifact (shared `db` + Notion connector). Opened as a plain file it runs in preview mode and stores data in localStorage only.

- Notion 과제 연동을 쓰려면 `index.html`의 `TASK_DS`를 본인 Notion 데이터 소스 주소로 바꾸세요.
- 방학·휴일 표시는 `SCHOOL_BREAKS`, 과제 분류별 색은 `CLASS_COLORS`, 블록 제목 → 타이머 과목 연결은 `PLAN_ALIASES`, 타이머 기본 과목은 `TM_DEFAULT`, 기본 블록 종류는 `DEFAULT_TYPES`에서 바꿉니다. 모두 빈 값/예시로 시작합니다.

개인 일정·계정 데이터는 이 저장소에 없습니다. 이름·과목·학교 일정·반복 블록·Notion 주소를 모두 비운 백지 상태이고, 블록 종류(잠·공부·휴식·운동)와 타이머 과목(Math·English·Science)은 예시입니다. 설정에서 직접 바꾸세요.
