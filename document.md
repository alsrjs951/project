# 프로젝트 기획 문서

## 기본 정보 (Basic Info)
- 프로젝트명: On-Device AI 민원 분석 및 처리 시스템
- 개요: 공공기관 폐쇄망 환경에서 민원 데이터를 안전하게 분석하고, 표준화된 답변 초안을 자동 생성하는 온프레미스 AI 시스템
- 동기: 민감한 민원 데이터의 보안 요구사항을 충족하면서도 민원 처리 속도와 품질을 동시에 높이기 위함
- 예상 결과물: 폐쇄망 내 설치 가능한 민원 분석/답변 생성 웹 서비스(모델, 서빙, UI 포함)

## 기술 스택 (Tech Stack)
- Frontend: Streamlit 기반 웹 UI
- Backend: Python 기반 데이터 처리 및 AI 추론 로직
- Database: 공개 민원/답변 데이터 저장용 DB(PostgreSQL 또는 MongoDB)
- Deployment: 폐쇄망 On-Premise 환경 + Docker 컨테이너 배포

## 주요 기능 (Key Features)
- 핵심 기능 1 (Core Feature): 지자체 전자민원창구 공개 데이터 수집 및 학습 데이터셋 구축
- 핵심 기능 2 (Core Feature): 오픈소스 sLLM(Gemma 2, Llama 3 등) 기반 SFT 학습과 표준 답변 초안 자동 생성
- 핵심 기능 3 (Core Feature): 폐쇄망 설치형 서비스 제공 및 Streamlit UI(입력, 생성, 수정, 복사) 지원

## 마일스톤 (Milestones)
- W 1-4: 요구사항 정의, 데이터 소스 선정, 크롤러/학습 환경 초기 세팅
- W 5-8: 데이터 수집 및 정제, SFT 학습, 답변 생성 MVP 구현
- W 9-12: 답변 품질 고도화, 온프레미스 성능 최적화, 기능 테스트
- W 13-16: Docker 패키징, 운영 문서화, 최종 검증 및 발표