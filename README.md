온마을 활동 코치
1) 간단한 소개
농촌 방과후 돌봄 현장에서 교사가

하루 프로젝트를 기획하고,
일지를 저장/검색하고,
보고서/TXT/PDF/시각자료를 만드는
웹 기반 프로토타입 앱입니다.
다로리 마을 맥락(자연·농업·공동체)을 반영해,
아이 활동 기획과 마을 커뮤니케이션(귀가 알림/이슈 벽)을 지원합니다.

2) 사용한 오픈소스 및 AI/출처
Tailwind CSS: https://github.com/tailwindlabs/tailwindcss
Lucide Icons: https://github.com/lucide-icons/lucide
Chart.js: https://github.com/chartjs/Chart.js
jsPDF: https://github.com/parallax/jsPDF
Compromise(NLP): https://github.com/spencermountain/compromise
(옵션) Flask/OpenAI/python-docx (서버 모드에서 사용)
이미지 소스(현재): Unsplash Source URL 기반 동적 로드

https://source.unsplash.com
3) 구현 방식 / 동작 원리
기본 모드: proto_1.html 단일 파일 SPA 방식 (탭 전환 UI)
데이터 저장: 브라우저 localStorage 사용
주요 기능:
로그인/계정 관리
프로젝트 기획(템플릿/직접작성)
일지 저장/검색
TXT/PDF 내보내기
시각자료(표/차트/관련 이미지)
귀가 알림 문구 생성
마을 이슈 벽
서버 모드 사용 시:
Flask(app.py)로 로컬 서버 실행
필요 시 OpenAI API 연동 가능

4) 실행 방법
A. 빠른 실행(권장, HTML만)
리포지토리 clone/download
proto_1.html 더블클릭
브라우저에서 바로 사용
B. Flask 실행(서버 모드)
프로젝트 폴더 이동
가상환경 생성/활성화
pip install -r requirements.txt
.env.example를 복사해 .env 생성 후 키 입력
python app.py
브라우저에서 http://127.0.0.1:5000 접속
