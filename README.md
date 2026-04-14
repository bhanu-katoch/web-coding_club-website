# 🎓 Club Hub — Student Club Management Platform

> A full-featured web platform for managing student club activities, events, merchandise, memberships, and open-source contributions.

---

## 📸 Overview

**Club Hub** is a modern, student-first web application designed to centralize everything a university club needs — from event registration and seat matrices to a merch store and GitHub project showcases. Built for engagement, transparency, and scale.

---

## 🗺️ Feature Screens

| # | Screen | Description |
|---|--------|-------------|
| 1 | 🏠 **Home** | News highlights, upcoming events feed, and a "Join Club" CTA |
| 2 | 📅 **Events List & Archive** | Browse upcoming events; explore past event photos, winners & reviews |
| 3 | 🪑 **Event Registration & Seat Matrix** | Register for events, view live seat availability map, get venue & result updates |
| 4 | 🛍️ **Merchandise Store** | Shop for club shirts & mugs; customize t-shirts with a live preview tool |
| 5 | 🤝 **Join / Volunteer** | Apply for club roles — design, event management, content, and more |
| 6 | 💻 **Projects & Contributions** | Discover active club projects with direct GitHub links for contributors |

---

## 🚀 Getting Started

### Prerequisites

- Node.js >= 18.x
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/your-org/club-hub.git
cd club-hub

# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be available at `http://localhost:3000`.

---

## 🧱 Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React / Next.js |
| Styling | Tailwind CSS |
| Backend | Node.js + Express (or Next.js API routes) |
| Database | PostgreSQL / Supabase |
| Auth | NextAuth.js / Clerk |
| Storage | Cloudinary (images), AWS S3 (assets) |
| Deployment | Vercel / Railway |

> ⚠️ Tech stack decisions are open for discussion. See [Issues](../../issues) for active proposals.

---

## 📁 Project Structure

```
club-hub/
├── public/               # Static assets
├── src/
│   ├── app/              # Next.js App Router pages
│   │   ├── page.tsx          # Home Screen
│   │   ├── events/           # Events List & Archive
│   │   ├── events/[id]/      # Event Registration & Seat Matrix
│   │   ├── store/            # Merchandise Store
│   │   ├── join/             # Join / Volunteer
│   │   └── projects/         # Projects & Contributions
│   ├── components/       # Shared UI components
│   ├── lib/              # Utilities, hooks, API helpers
│   └── styles/           # Global styles
├── prisma/               # DB schema (if using Prisma)
├── .env.example          # Environment variable template
└── README.md
```

---

## 🌿 Branching Strategy

```
main          → Production-ready code
dev           → Integration branch for features
feature/*     → Individual feature branches
fix/*         → Bug fix branches
```

**Branch naming examples:**
- `feature/seat-matrix-ui`
- `feature/merch-customizer`
- `fix/event-registration-form`

---

## 🤝 Contributing

We welcome contributions from club members and the open-source community!

1. Fork the repo
2. Create your branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "feat: add seat matrix component"`
4. Push: `git push origin feature/your-feature`
5. Open a **Pull Request** against `dev`

Please read [CONTRIBUTING.md](./CONTRIBUTING.md) before submitting PRs.

---

## 🐛 Reporting Issues

Found a bug or have a feature request? [Open an issue](../../issues/new) using one of our templates:
- 🐛 Bug Report
- ✨ Feature Request
- 📋 Screen / UI Task
- ❓ Question

---

## 📜 License

This project is licensed under the [MIT License](./LICENSE).

---

## 👥 Maintainers

| Role | Name | GitHub |
|------|------|--------|
| Project Lead | Bhanu Katoch | @bhanu-katoch |
| Design | — | @handle |
| Backend | — | @handle |

---

> Built with ❤️ by the club community. Star ⭐ the repo if you find it useful!