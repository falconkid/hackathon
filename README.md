```markdown
# HireIQ — Prototype

Quick start (local):

1. Backend
- cd backend
- copy .env.example -> .env and fill OPENAI_API_KEY (and optional Firebase)
- npm install
- npm run dev

2. Frontend
- cd frontend
- copy .env.example -> .env.local and set VITE_API_BASE to your backend URL (e.g. http://localhost:4000)
- npm install
- npm run start

Notes:
- This prototype uses an in-memory store for interviews in the backend for quick demo. Replace with Firebase in backend/src/services/firebaseAdmin.js for persistence.
- Camera uses a minimal CameraView component. Swap to face-api.js: load models and compute expressions in CameraView.
- Speech uses the Web Speech API; switch to Whisper/Whisper API for server-side transcription if needed.
- Keep OpenAI keys server-side (in backend .env).
```