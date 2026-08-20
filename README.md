# StoryBoardMaker

시나리오 텍스트를 AI가 씬·샷 단위로 분해하고, 각 컷을 이미지로 자동 생성해 프로덕션급 스토리보드를 만들어주는 서비스입니다.

기획 배경과 전체 로드맵은 [storyboard_service_plan.md](./storyboard_service_plan.md) 참고.

## 프로젝트 구조

```
StoryBoardMaker/
├── frontend/   # Next.js (React, TypeScript, App Router, Tailwind CSS)
└── backend/    # NestJS (TypeScript)
```

## 시작하기

### Frontend

```bash
cd frontend
npm run dev
```

http://localhost:3000 에서 확인할 수 있습니다.

### Backend

```bash
cd backend
npm run start:dev
```

http://localhost:4000 에서 API 서버가 실행됩니다.

## 기술 스택

- **Frontend**: Next.js, React, TypeScript, Tailwind CSS
- **Backend**: NestJS, TypeScript

자세한 기능 및 아키텍처 계획은 [storyboard_service_plan.md](./storyboard_service_plan.md)를 참고하세요.
