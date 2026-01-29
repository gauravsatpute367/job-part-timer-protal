# PartTimer — Frontend (React + Vite)

This folder contains the **PartTimer** frontend built with **React**, **React Router**, **Tailwind CSS**, and **Vite**.

## Prerequisites

- Node.js (LTS recommended)
- Backend API running (see the root [setup.md](../setup.md))

Default local URLs:

- Frontend (Vite): `http://localhost:5173`
- Backend API: `http://localhost:5000`

## Run locally

From this `frontend/` folder:

```powershell
npm install
npm run dev
```

## Build + lint

```powershell
npm run build
npm run lint
```

## Auth storage (browser)

After login, the frontend stores these values in `localStorage`:

- `token`
- `role`
- `userName`
- `userId`

## Key folders

- `src/pages/` — route pages (admin, auth, dashboard, employer, jobs, jobseeker)
- `src/components/` — shared UI components
- `src/utils/` — small utilities (auth/date helpers)

## Notable routes (implemented)

- Admin:
  - `/admin/employers`, `/admin/jobseekers`, `/admin/activities`
  - `/admin/jobs` (All Jobs)
  - `/admin/applications` (All Applications)
- Employer:
  - `/employer/my-jobs`, `/employer/applications`, `/employer/jobs/:jobId/applications`
- Jobseeker:
  - `/jobseeker/my-applications`

## Profile uploads

- Profile photo upload is supported.
- Jobseeker resume upload is supported (PDF), stored as a file on the backend and linked from profile pages.

For a full feature + API overview, see the root [PARTTIMER_SYSTEM_GUIDE.md](../PARTTIMER_SYSTEM_GUIDE.md).
