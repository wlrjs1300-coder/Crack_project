🏗️ CRACK: 도로 파손 실시간 AI 탐지 및 시민 참여형 제보 플랫폼
CRACK은 시민들의 자발적인 제보와 실시간 AI 분석 기술을 결합하여, 포트홀 및 싱크홀과 같은 도로 파손 위험을 신속하게 관리자에게 전달하는 스마트 시티 솔루션입니다.


🌟 핵심 기능 (Key Features)
1. 지능형 AI 제보 시스템 (report_service.py)
멀티미디어 분석: 사진뿐만 아니라 동영상 제보 시 프레임별 분석을 통해 도로 파손 위치를 정밀 탐지합니다.

YOLOv8 기반 자동 검증: 제보된 파일은 서버에서 실시간으로 분석되며, 포트홀(신뢰도 60% 이상) 또는 싱크홀 감지 시에만 승인됩니다.

자동 위치 추출 (EXIF & Reverse Geocoding): 사진의 메타데이터에서 GPS 좌표를 자동 추출하고, Kakao Map API를 통해 도로명 주소로 변환합니다.

2. 실시간 관리자 관제 시스템 (admin_service.py)
Live Dashboard: Socket.io를 활용하여 새로운 위험 요소 발견 시 관리자에게 즉각적인 브라우저 푸시 알림을 제공합니다.

데이터 시각화: Chart.js를 통해 지역별 위험도 순위, 시계열별 사고 발생 추이를 직관적인 통계 화면으로 제공합니다.

위험도 점수(Risk Score): AI가 판단한 객체의 크기와 신뢰도를 기반으로 사고의 긴급도를 수치화합니다.

3. 사용자 참여 및 보상 체계 (my_service.py)
크래커 포인트(Point System): 유효한 제보 완료 시 포인트를 지급하여 시민들의 지속적인 참여를 유도합니다.

실시간 상태 확인: 내가 신고한 도로의 처리 과정(AI 분석중 -> 관리자 확인중 -> 처리중 -> 완료)을 실시간으로 추적할 수 있습니다.

4. 고도화된 보안 및 데이터 관리
비속어 필터링: 자체 구축한 profanity.json 기반의 헥사 코드 필터링으로 클린한 커뮤니티 환경을 유지합니다.

데이터 정합성: migrate_db.py 및 rollback_db.py를 통해 안전한 데이터베이스 이관 및 복구 프로세스를 구축했습니다.


보내주신 모든 소스 코드를 종합하여, CRACK(도로 파손 실시간 탐지 및 신고 서비스) 프로젝트의 기술적 강점과 UI/UX 디자인 철학이 돋보이는 README를 작성해 드립니다.

🏗️ CRACK: 도로 파손 실시간 AI 탐지 및 시민 참여형 제보 플랫폼
CRACK은 시민들의 자발적인 제보와 실시간 AI 분석 기술을 결합하여, 포트홀 및 싱크홀과 같은 도로 파손 위험을 신속하게 관리자에게 전달하는 스마트 시티 솔루션입니다.

🌟 핵심 기능 (Key Features)
1. 지능형 AI 제보 시스템 (report_service.py)
멀티미디어 분석: 사진뿐만 아니라 동영상 제보 시 프레임별 분석을 통해 도로 파손 위치를 정밀 탐지합니다.

YOLOv8 기반 자동 검증: 제보된 파일은 서버에서 실시간으로 분석되며, 포트홀(신뢰도 60% 이상) 또는 싱크홀 감지 시에만 승인됩니다.

자동 위치 추출 (EXIF & Reverse Geocoding): 사진의 메타데이터에서 GPS 좌표를 자동 추출하고, Kakao Map API를 통해 도로명 주소로 변환합니다.

2. 실시간 관리자 관제 시스템 (admin_service.py)
Live Dashboard: Socket.io를 활용하여 새로운 위험 요소 발견 시 관리자에게 즉각적인 브라우저 푸시 알림을 제공합니다.

데이터 시각화: Chart.js를 통해 지역별 위험도 순위, 시계열별 사고 발생 추이를 직관적인 통계 화면으로 제공합니다.

위험도 점수(Risk Score): AI가 판단한 객체의 크기와 신뢰도를 기반으로 사고의 긴급도를 수치화합니다.

3. 사용자 참여 및 보상 체계 (my_service.py)
크래커 포인트(Point System): 유효한 제보 완료 시 포인트를 지급하여 시민들의 지속적인 참여를 유도합니다.

실시간 상태 확인: 내가 신고한 도로의 처리 과정(AI 분석중 -> 관리자 확인중 -> 처리중 -> 완료)을 실시간으로 추적할 수 있습니다.

4. 고도화된 보안 및 데이터 관리
비속어 필터링: 자체 구축한 profanity.json 기반의 헥사 코드 필터링으로 클린한 커뮤니티 환경을 유지합니다.

데이터 정합성: migrate_db.py 및 rollback_db.py를 통해 안전한 데이터베이스 이관 및 복구 프로세스를 구축했습니다.

🛠 Tech Stack
Backend
Framework: Flask (Python)

Database: MySQL (MariaDB compatible), Flask-SQLAlchemy (ORM)

AI Model: YOLOv8 (Ultralytics)

Real-time: Flask-SocketIO (WebSocket)

Frontend
Template Engine: Jinja2

UI Framework: Bootstrap 5, Custom CSS3 (Modern Glassmorphism Design)

Typography: Outfit (Heading), Inter (Body)

Map Service: Kakao Maps API / Leaflet (Mobile optimized)



📁 Project Structure
├── app.py              # Flask Application Entry Point
├── models.py           # Database Models (Member, Report, AiResult etc.)
├── extensions.py       # Flask Extensions (DB, SocketIO)
├── utils.py            # Helpers (EXIF Extraction, Profanity Filter, Geocoding)
├── services/           # Business Logic Blueprints
│   ├── admin_service.py
│   ├── auth_service.py
│   ├── report_service.py
│   └── status_service.py
├── templates/          # HTML Templates (Responsive Mobile & Admin Desktop)
├── secrets/            # Config Files (.env, profanity.json - Git Ignored)
└── uploads/            # User-Uploaded Media (Images/Videos)


🚀 Installation & Setup
1. 가상환경 구성 및 패키지 설치
  python -m venv .venv
  source .venv/bin/activate  # Windows: .venv\Scripts\activate
  pip install -r requirements.txt

2. 환경 변수 설정 (secrets/.env 파일을 생성하고)
  DB_HOST=your_host
  DB_USER=your_user
  DB_PASSWORD=your_password
  KAKAO_REST_API_KEY=your_kakao_key

3. 서버 실행
  # 전용 배치 파일 실행 또는 명령행 실행
  run_server.bat
  # 또는
  python app.py


🎨 UI/UX Design Identity
* Primary Color: #FF8C00 (Safety Orange) - '주의'와 '안전'을 상징
* Surface: Semi-transparent Glassmorphism
* Concept: 모바일에서는 직관적인 제보 경험을, 데스크톱(관리자)에서는 방대한 데이터를 효율적으로 처리할 수 있는 대시보드 인터페이스를 제공합니다.
