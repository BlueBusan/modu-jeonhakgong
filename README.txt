모두의 전학공 찾기 v2 - Firebase 설정

1. Firebase Console > Authentication > Sign-in method > Anonymous(익명) 활성화
2. Firestore Database가 없다면 생성
3. firestore.rules를 프로젝트에 배포
   firebase login
   firebase use modu-jeonhakgong
   firebase deploy --only firestore:rules
4. modu-schedule-v2.html을 GitHub Pages의 index.html로 배포
5. 최초 접속 시 URL에 ?room=room_... 이 자동으로 붙는지 확인
6. '방 링크 복사'로 복사한 동일 링크를 다른 브라우저/휴대폰에서 열기
7. 상단 상태가 연결됨/동기화됨/저장됨으로 표시되는지 확인

주의: 현재 규칙은 '익명 로그인한 사용자가 방 ID를 알면 읽기/쓰기 가능'한 소규모 링크 공유형입니다. 개인정보/민감정보 저장 용도로는 사용하지 마세요.
