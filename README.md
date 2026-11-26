# GEO 진단 사이트

## 파일 구성
- server.ts : 서버. 화면에서 받은 영상을 Gemini에 보내고 점수를 계산해 돌려줌 (API 키는 여기서만 사용)
- src/App.tsx : 화면 (탭, 입력창, 결과 표시)
- src/geoCriteria.ts : GEO 진단 기준 11개, Gemini에 보내는 지시문, 점수 계산 규칙
- src/mockResult.ts : 테스트용 예시 결과 (MOCK_GEMINI=1 일 때 사용)
- .env.example : 내 컴퓨터에서 실행할 때 쓰는 설정 예시

## 내 컴퓨터에서 실행
1. npm install
2. .env.example 을 복사해 .env 로 이름 변경 후 GEMINI_API_KEY 입력
3. npm run local → 브라우저에서 http://localhost:3000
