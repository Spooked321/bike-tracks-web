# Bike Tracks Web

## What this is
React + TypeScript web frontend for a bike tracking app with NFC tagging and stolen bike reporting.
This is one of 3 repos in the project (api / web / mobile).

## Stack
- **Framework**: React 18 + TypeScript
- **Build/Deploy**: Vite + Vercel
- **Auth**: Firebase Auth
- **Styling**: Tailwind CSS
- **API client**: fetch / React Query (TBD)
- **Testing**: Vitest + React Testing Library

## Project phases
- [ ] Phase 1–4: (Backend — separate repo, must be done first)
- [ ] Phase 5: Web Frontend ← THIS REPO
  - Auth flow (login / register)
  - My bikes dashboard
  - Register a bike
  - Report stolen / mark recovered
  - Search stolen bikes

## Folder structure (target)
```
bike-tracks-web/
├── src/
│   ├── main.tsx
│   ├── App.tsx
│   ├── pages/           # Route-level components
│   ├── components/      # Reusable UI components
│   ├── hooks/           # Custom hooks (useAuth, useBikes etc.)
│   ├── api/             # API call functions
│   ├── types/           # Shared TypeScript types
│   └── lib/             # Firebase config, utils
├── public/
├── .env.example
├── index.html
└── PROJECT_STATUS.md
```

## Working rules
- Keep it simple — no premature abstraction
- TypeScript strict mode — no `any` unless truly necessary
- Mobile-first responsive design
- Never commit real credentials — use .env files
- Update PROJECT_STATUS.md after completing each phase
- Ask before adding new dependencies

## Environment variables needed
```
VITE_API_URL=http://localhost:8000
VITE_FIREBASE_API_KEY=your-key
VITE_FIREBASE_AUTH_DOMAIN=your-project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your-project-id
```

## Key commands
```bash
npm run dev      # Start dev server
npm run build    # Production build
npm run test     # Run tests
npm run lint     # Lint check
```
