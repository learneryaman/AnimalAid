AnimalAid — Rescue → Treatment → Release (People • NGO/Hospital • Admin)
AnimalAid is a ready-to-use single-page web prototype that helps citizens report injured/stray animals, enables NGOs/Government hospitals to manage rescue and treatment checkpoints, and provides transparent, downloadable treatment reports.

Key Features
People Portal

Google-style login (demo fallback if Firebase not configured)
Camera capture or image upload
Browser geolocation auto-fill (no location APIs)
Optional AI-assisted triage (symptoms → likely issues, urgency, safe next steps)
Request tracking with unique token + checkpoint timeline:
Requested → Captured → Treatment Done → Released
Completed treatment reports with PDF download
NGO / Government Hospital Portal

Email/Password login (demo fallback)
View and operate today’s requests
Update checkpoints (Captured / Treated / Released)
Edit treatment report: cause, time taken, summary
Weekly/monthly analytics + PDF export
Admin Portal

Oversight dashboard with stage KPIs
Export/Import requests as JSON
Clear local data
PDF summary export
AI Integration (Optional)
Supports “bring your own OpenAI API key” for:

Triage suggestions from text (and image, if provided)
Complaint/report drafting
Treatment report summarization
Chat-like helper inside the app
If no key is set, the app uses a local heuristic fallback.
Data Persistence
Works out of the box using localStorage (demo mode).
Can be extended to Firebase Auth + Firestore in production (not required for demo recording).
Demo Mode (For Video Recording)
Includes a One-click Demo Studio to:

Open People / NGO / Admin demo portals instantly
Seed sample requests (including completed cases for PDF demo)
Clear all requests for a fresh run
Tech Stack
Single-page app: HTML + TailwindCSS + Vanilla JavaScript
PDFs: jsPDF
Optional auth/persistence: Firebase Auth / Firestore (when configured)
Optional AI: OpenAI Chat Completions API
Use Cases
Citizen reporting + location-aware dispatch
Transparent rescue/treatment tracking
Verified release reports with shareable PDFs
NGO workload reporting and analytics
