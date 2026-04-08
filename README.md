# MovieHorizon

<div align="center">
	<img src="./src/assets/white-logo.svg" alt="MovieHorizon Logo" width="220" />
	<h3>Explore movies, actors and details in a cinematic, responsive experience.</h3>

	<p>
		<img src="https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React" />
		<img src="https://img.shields.io/badge/TypeScript-5.8-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
		<img src="https://img.shields.io/badge/Vite-7-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
		<img src="https://img.shields.io/badge/TailwindCSS-4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind" />
		<img src="https://img.shields.io/badge/Firebase-Auth-FFCA28?style=flat-square&logo=firebase&logoColor=black" alt="Firebase" />
		<img src="https://img.shields.io/badge/TMDB-API-01D277?style=flat-square" alt="TMDB" />
	</p>
</div>

---

## 🚀 Demo

> Add your deployed URL here when ready.

- Production: Pending
- Storybook: Run locally with `npm run storybook`

---

## 🧠 Overview

MovieHorizon is a web app focused on movie discovery with a polished UI and smooth navigation between:

- Popular movies list (infinite scrolling)
- Movie detail pages with cast and production data
- Actor detail pages with filmography
- Authentication with Firebase (email/password + Google)
- Guest mode access to reduce user friction

---

## 🏗️ Architecture

The project is organized into clear layers and feature modules:

### 🔷 Presentation Layer

- Reusable UI components and feature blocks
- Route-based pages for each user flow
- Tailwind-powered responsive layouts

### 🔷 Data Layer

- TMDB data requests via Axios
- Server-state management with TanStack Query
- Typed models for API payloads

### 🔷 Auth Layer

- Firebase Auth provider and auth service
- Protected routes for private pages
- Guest session mode with session storage

---

## 📂 Project Structure

```text
src/
├── auth/
│   ├── components/
│   ├── context/
│   └── hooks/
├── components/
│   ├── animations/
│   ├── audio/
│   ├── Button/
│   ├── Card/
│   └── Logo/
├── config/
│   └── tmdb.ts
├── features/
│   ├── footer/
│   ├── header/
│   └── main/
├── pages/
│   ├── actorDetailsPage/
│   ├── loginPage/
│   ├── movieDetailsPage/
│   ├── moviePage/
│   ├── registerPage/
│   └── welcomePage/
├── routes/
└── types/
```

---

## ✨ Core Features

### 🔐 Authentication

- Register and login with email/password
- Google sign-in
- Route protection for private sections
- Guest access flow from Login page

### 🎬 Movie Discovery

- Popular movies feed from TMDB
- Infinite scroll using IntersectionObserver
- Card-based browsing UI

### 🎥 Movie Details

- Poster, backdrop and metadata
- Runtime, release date, revenue, genres
- Cast and crew references

### 🎭 Actor Details

- Actor profile information
- Filmography list
- Easy navigation between actor and movie pages

### 🎵 Ambient Experience

- Optional audio player component when authenticated

---

## 🧪 Technologies Used

- React 19
- TypeScript
- Vite
- Tailwind CSS v4
- TanStack Query
- React Router
- Firebase Auth
- Axios
- Storybook
- ESLint

---

## ⚙️ Setup & Installation

### 1) Clone and install

```bash
git clone <your-repository-url>
cd MovieApp-v2
npm install
```

### 2) Environment variables

Create a `.env` file in the project root:

```env
VITE_TMDB_API_KEY=your_tmdb_api_key

VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
VITE_FIREBASE_PROJECT_ID=your_firebase_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
VITE_FIREBASE_APP_ID=your_firebase_app_id
```

### 3) Run locally

```bash
npm run dev
```

Open: `http://localhost:5173`

---

## 📜 Available Scripts

- `npm run dev` Starts local dev server
- `npm run build` Builds production bundle
- `npm run preview` Serves built app locally
- `npm run lint` Runs ESLint
- `npm run storybook` Starts Storybook
- `npm run build-storybook` Builds Storybook static bundle
- `npm run deploy` Deploys to GitHub Pages (after build)

---

## 🧭 Navigation Flow

1. Welcome page
2. Login or register (or continue as guest)
3. Movies list
4. Movie details
5. Actor details

---

## 🔒 Security Notes

- API keys are read from environment variables
- Auth state is managed centrally through context
- Protected routes block non-authenticated/non-guest users

---

## 📌 Roadmap

- Favorites and watchlist persistence
- Search and filtering improvements
- Better user profile and preferences
- Optional dark/light theme switcher

---

## 👨‍💻 Author

Built by MovieHorizon Team.
