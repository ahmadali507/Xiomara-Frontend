<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:6D28D9,40:A855F7,80:EC4899,100:F43F5E&height=220&section=header&text=Xiomara&fontSize=85&fontColor=ffffff&fontAlignY=38&desc=AI-Powered%20Content%20Marketing%20Platform&descAlignY=58&descSize=22&animation=fadeIn" width="100%"/>
</p>

<p align="center">
  <a href="https://github.com/ahmadali507/Xiomara-Frontend">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=A855F7&center=true&vCenter=true&width=750&lines=AI-Powered+Content+Generation+Engine;Multi-Client+%7C+Multi-Campaign+Management;Bilingual+%7C+English+%26+Spanish;Built+with+Next.js+15+%2B+TypeScript+%2B+Tailwind+v4" alt="Typing SVG" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Next.js-15.5-black?style=for-the-badge&logo=next.js&logoColor=white"/>
  <img src="https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind_CSS-v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
  <img src="https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/shadcn%2Fui-latest-18181B?style=for-the-badge&logo=shadcnui&logoColor=white"/>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/i18n-EN%20%7C%20ES-A855F7?style=flat-square"/>
  <img src="https://img.shields.io/badge/TanStack_Query-v5-FF4154?style=flat-square&logo=reactquery&logoColor=white"/>
  <img src="https://img.shields.io/badge/React_Hook_Form-+_Zod-EC4899?style=flat-square"/>
  <img src="https://img.shields.io/badge/App_Router-SSR%20%2B%20Server_Actions-black?style=flat-square&logo=next.js"/>
  <img src="https://img.shields.io/badge/License-MIT-22C55E?style=flat-square"/>
</p>

<br/>

<p align="center">
  <b>Xiomara</b> is a full-stack, bilingual content marketing platform that gives agencies and teams a single workspace to manage clients, run campaigns, ingest information sources, generate AI-powered summaries, and produce publication-ready content outputs — all from one structured, multi-tenant interface.
</p>

---

## 📋 Table of Contents

<p align="center">
  <a href="#-overview"><img src="https://img.shields.io/badge/Overview-6D28D9?style=flat-square"/></a>
  <a href="#-features"><img src="https://img.shields.io/badge/Features-A855F7?style=flat-square"/></a>
  <a href="#%EF%B8%8F-tech-stack"><img src="https://img.shields.io/badge/Tech%20Stack-EC4899?style=flat-square"/></a>
  <a href="#-architecture"><img src="https://img.shields.io/badge/Architecture-F43F5E?style=flat-square"/></a>
  <a href="#-project-structure"><img src="https://img.shields.io/badge/Structure-EF4444?style=flat-square"/></a>
  <a href="#-getting-started"><img src="https://img.shields.io/badge/Getting%20Started-22C55E?style=flat-square"/></a>
  <a href="#-environment-variables"><img src="https://img.shields.io/badge/Env%20Vars-F59E0B?style=flat-square"/></a>
  <a href="#-core-modules"><img src="https://img.shields.io/badge/Core%20Modules-0EA5E9?style=flat-square"/></a>
  <a href="#-routing--i18n"><img src="https://img.shields.io/badge/Routing%20%26%20i18n-9CA3AF?style=flat-square"/></a>
  <a href="#-contributing"><img src="https://img.shields.io/badge/Contributing-16A34A?style=flat-square"/></a>
</p>

---

## 🔍 Overview

Xiomara is built for content and marketing agencies that manage multiple clients and campaigns simultaneously. The platform follows a hierarchical data model:

```
Agency (Platform)
 └── Clients          (brands, companies, or accounts)
      └── Campaigns   (specific marketing initiatives per client)
           ├── Fuentes          (information sources: articles, docs, URLs)
           ├── Knowledge Base   (curated reference documents)
           ├── Media            (image and media assets)
           ├── Corresponsables  (Telegram listeners & co-owners)
           └── Content Engine   (AI pipeline: sources → summary → output)
```

The **Content Engine** is the core AI feature. It lets users select sources, generate an AI summary from them using configurable templates, and produce structured content outputs ready for publishing — all within the same scoped workspace (client or campaign).

---

## ✨ Features

<table>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%94%90-Authentication_System-6D28D9?style=for-the-badge"/><br/>
      <sub>Full auth flow: login, signup, forgot password, reset password, and an admin-approval pending state. Token stored as a secure httpOnly cookie.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%8F%A2-Client_Management-A855F7?style=for-the-badge"/><br/>
      <sub>Create, edit, and delete clients with industry, contact info, brand guide, logo, and WhatsApp. Each client has its own scoped workspace.</sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%93%85-Campaign_Management-EC4899?style=for-the-badge"/><br/>
      <sub>Create campaigns nested under clients with name, type, start date, and description. All sub-features (fuentes, knowledge, media) are campaign-scoped.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%A4%96-Content_Engine_(AI)-F43F5E?style=for-the-badge"/><br/>
      <sub>Three-step AI pipeline: select sources → generate summaries → produce template-based outputs. Supports iterative refinement and output editing.</sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%93%B0-Fuentes_(Sources)-EF4444?style=for-the-badge"/><br/>
      <sub>Ingest information from URLs, documents, and other source types. Sources are folder-scoped and selectable inside the Content Engine.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%93%9A-Knowledge_Base-F97316?style=for-the-badge"/><br/>
      <sub>Upload and manage reference documents for each client or campaign. Used to provide background context during AI content generation.</sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%96%BC%EF%B8%8F-Media_Management-F59E0B?style=for-the-badge"/><br/>
      <sub>Upload, organize, and attach image and media assets scoped to a client or campaign. Includes a media post preview component.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%93%A1-Corresponsables-22C55E?style=for-the-badge"/><br/>
      <sub>Connect Telegram listeners and assign co-responsible team members to clients and campaigns, with a dedicated token dialog.</sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%8C%90-Bilingual_(EN%2FES)-06B6D4?style=for-the-badge"/><br/>
      <sub>Full internationalization via next-intl. Spanish is the default locale. All UI strings are managed through en.json and es.json message files.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%94%97-Shareable_Links-0EA5E9?style=for-the-badge"/><br/>
      <sub>Generate shareable links for client workspaces and campaign outputs, with a dedicated share dialog and link copy functionality.</sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/%F0%9F%93%9D-Templates-9333EA?style=for-the-badge"/><br/>
      <sub>Create global and user-specific prompt templates that drive the AI output generation step. Templates are reusable across any campaign.</sub>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/%E2%9C%85-Admin_Panel-16A34A?style=for-the-badge"/><br/>
      <sub>Admin-only actions for managing users and approving newly registered accounts before they can access the platform.</sub>
    </td>
  </tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

### Frontend & Framework

| Technology | Version | Purpose |
|:---|:---:|:---|
| [Next.js](https://nextjs.org/) | 15.5.0 | React framework with App Router, SSR, and Server Actions |
| [React](https://react.dev/) | 18.3.1 | UI library |
| [TypeScript](https://www.typescriptlang.org/) | 5.x | Static typing across the entire codebase |
| [Tailwind CSS](https://tailwindcss.com/) | v4 | Utility-first styling with `tw-animate-css` for animations |

### State, Data & Forms

| Technology | Version | Purpose |
|:---|:---:|:---|
| [TanStack Query](https://tanstack.com/query) | v5 | Server state management, caching, and background refetch |
| [React Hook Form](https://react-hook-form.com/) | 7.62.0 | Performant form state management |
| [Zod](https://zod.dev/) | 4.x | Schema validation for all form inputs and API responses |
| [Axios](https://axios-http.com/) | 1.11.0 | HTTP client used within Server Actions |

### UI & Components

| Technology | Version | Purpose |
|:---|:---:|:---|
| [shadcn/ui](https://ui.shadcn.com/) | latest | Pre-built accessible component library |
| [Radix UI](https://www.radix-ui.com/) | various | Headless primitives (Dialog, Dropdown, Avatar, Checkbox, Popover, Select) |
| [Lucide React](https://lucide.dev/) | 0.541.0 | Comprehensive icon set |
| [Sonner](https://sonner.emilkowal.ski/) | 2.0.7 | Toast notification system |
| [React Quill New](https://github.com/VaguelySerious/react-quill) | 3.6.0 | Rich text editor for content creation |
| [next-themes](https://github.com/pacocoursey/next-themes) | 0.4.6 | Light/dark theme management |
| [class-variance-authority](https://cva.style/) | 0.7.1 | Variant-based component styling |

### Internationalization & Auth

| Technology | Version | Purpose |
|:---|:---:|:---|
| [next-intl](https://next-intl-docs.vercel.app/) | 4.3.5 | Full i18n with locale routing, messages, and middleware |
| [cookies-next](https://github.com/andreizanik/cookies-next) | 6.1.0 | Cookie management for auth tokens |

</div>

---

## 🏗️ Architecture

```
╔════════════════════════════════════════════════════════════════════╗
║                    XIOMARA — SYSTEM ARCHITECTURE                   ║
╚════════════════════════════════════════════════════════════════════╝

 Browser Client
       │
       ▼
 ┌─────────────────────────────────────────────────────────────┐
 │                  Next.js 15 App (App Router)                 │
 │                                                              │
 │  ┌─────────────────┐      ┌──────────────────────────────┐  │
 │  │ next-intl        │      │      Middleware               │  │
 │  │ Middleware       │      │  • Locale detection & routing │  │
 │  │ /en/  or  /es/  │      │  • Auth token guard           │  │
 │  └─────────────────┘      │  • Client selection guard     │  │
 │                            └──────────────────────────────┘  │
 │                                                              │
 │  ┌──────────────────────────────────────────────────────┐   │
 │  │               Page / Layout Layer                    │   │
 │  │  app/[locale]/auth/*        (login, signup, reset)   │   │
 │  │  app/[locale]/clients/*     (client & campaign pages)│   │
 │  └──────────────────────────────────────────────────────┘   │
 │                                                              │
 │  ┌──────────────────────────────────────────────────────┐   │
 │  │            React Context + TanStack Query             │   │
 │  │  AuthContext      ClientContext    TemplatesContext   │   │
 │  └──────────────────────────────────────────────────────┘   │
 │                                                              │
 │  ┌──────────────────────────────────────────────────────┐   │
 │  │              Next.js Server Actions                   │   │
 │  │  auth    clients    campaigns    knowledge            │   │
 │  │  sources    outputs    summaries    templates         │   │
 │  │  corresponsables    images    admin                   │   │
 │  └──────────────────────────────────────────────────────┘   │
 └─────────────────────────────────────────────────────────────┘
                              │
                              │  Axios (HTTP) via Server Actions
                              ▼
                  ┌───────────────────────┐
                  │    External Backend    │
                  │  REST API (Port 8888)  │
                  │  Auth, AI Engine,      │
                  │  File Storage, Folders │
                  └───────────────────────┘
```

---

## 📁 Project Structure

```
Xiomara-Frontend/
│
├── 📂 app/[locale]/                     # Internationalized App Router pages
│   ├── 🔐 auth/
│   │   ├── login/page.tsx               # Login page
│   │   ├── signup/page.tsx              # Registration page
│   │   ├── forgot-password/page.tsx     # Password recovery
│   │   ├── reset-password/page.tsx      # Password reset (token)
│   │   └── pending/page.tsx             # Awaiting admin approval
│   ├── 🏢 clients/
│   │   ├── page.tsx                     # All clients dashboard
│   │   ├── layout.tsx                   # Client layout with shared nav
│   │   └── [clientId]/
│   │       ├── page.tsx                 # Single client overview
│   │       ├── content-engine/          # Client-level content engine
│   │       ├── fuentes/                 # Client-level sources
│   │       ├── knowledge/               # Client-level knowledge base
│   │       ├── media/                   # Client-level media
│   │       ├── corresponsables/         # Client-level co-responsibles
│   │       └── campaigns/[campaignId]/  # All sections scoped to campaign
│   │           ├── page.tsx             # Campaign overview
│   │           ├── content-engine/      # Campaign content engine
│   │           ├── fuentes/             # Campaign sources
│   │           ├── knowledge/           # Campaign knowledge base
│   │           ├── media/               # Campaign media
│   │           └── corresponsables/     # Campaign co-responsibles
│   ├── globals.css                      # Global styles + Tailwind directives
│   ├── layout.tsx                       # Root layout with providers
│   └── page.tsx                         # Root redirect page
│
├── 📂 actions/                          # Next.js Server Actions
│   ├── auth.ts                          # login, signup, logout, profile, password reset
│   ├── clients.ts                       # CRUD for client folders
│   ├── campaigns.ts                     # CRUD for campaign folders
│   ├── sources.ts                       # Source ingestion and management
│   ├── knowledge.ts                     # Knowledge base documents
│   ├── summaries.ts                     # AI summary generation & editing
│   ├── outputs.ts                       # AI output generation from templates
│   ├── templates.ts                     # Prompt template management
│   ├── corresponsables.ts               # Telegram listeners & co-owners
│   ├── images.ts                        # Image upload and management
│   ├── admin.ts                         # Admin user management
│   └── _folders.ts                      # Internal folder utility helpers
│
├── 📂 components/
│   ├── 🔐 auth/                         # Login, Signup, ForgotPassword, ResetPassword forms
│   ├── 🏢 clients/                      # Client cards, forms, tabs, campaign rows
│   ├── 📊 dashboard/                    # Campaign dashboard: metrics, fuentes, media, knowledge cards
│   ├── 🤖 content-engine/               # Chat card, fuentes card, output card, post editor, edit form
│   ├── 💬 dialogs/                      # ShareLink, SummariesView, SummarySelection dialogs
│   ├── 📄 pages/                        # Top-level page wrapper components
│   ├── 🏗️ providers/                    # ClientOnly, QueryProvider
│   ├── ⏳ skeletons/                    # Loading skeleton components for all auth forms
│   └── 🎨 ui/                           # Shared UI: button, card, input, table, dialog,
│                                        #   rich-text-editor, metric-card, media-post, pagination…
│
├── 📂 context/
│   ├── AuthContext.tsx                  # Global auth state, user profile, logout
│   ├── ClientContext.tsx                # Selected client and campaign state
│   └── TemplatesContext.tsx             # Global templates list for content engine
│
├── 📂 hooks/
│   ├── useClients.ts                    # Client fetch, create, delete with React Query
│   ├── useCorresponsables.ts            # Corresponsables CRUD
│   ├── useKnowledge.ts                  # Knowledge base CRUD
│   ├── useSources.ts                    # Sources CRUD
│   ├── useSharing.ts                    # Share link generation
│   ├── useDataWithCache.ts              # Generic caching hook
│   └── usePagination.ts                 # Client-side pagination helper
│
├── 📂 lib/
│   ├── types.ts                         # Global TypeScript interfaces (User, AuthContextType, ApiResponse)
│   ├── schemas.ts                       # Zod schemas for all forms and API responses
│   ├── routes.ts                        # Centralized route constants and helpers
│   ├── api.ts                           # Axios base instance configuration
│   ├── utils.ts                         # Shared utility functions (cn, formatDate, etc.)
│   ├── dataPersistence.ts               # Cookie-based client/campaign persistence
│   └── withAuth.tsx                     # HOC for route-level auth protection
│
├── 📂 i18n/
│   ├── routing.ts                       # Locale list: ['en', 'es'], defaultLocale: 'es'
│   ├── navigation.ts                    # i18n-aware navigation helpers
│   └── request.ts                       # Server-side locale resolution
│
├── 📂 messages/
│   ├── en.json                          # English UI strings
│   └── es.json                          # Spanish UI strings (default locale)
│
├── 📂 utils/
│   ├── pagination.ts                    # Pagination math utilities
│   └── types.ts                         # Shared utility types
│
├── middleware.ts                        # i18n routing + auth guard + client selection guard
├── next.config.ts                       # Next.js configuration
├── components.json                      # shadcn/ui component registry config
├── tsconfig.json                        # TypeScript configuration
└── package.json
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- **Node.js** `>= 18.x`
- **npm** `>= 9.x` (or `pnpm` / `yarn`)
- The **Xiomara backend** running and accessible (defaults to `http://localhost:8888`)

---

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/ahmadali507/Xiomara-Frontend.git
cd Xiomara-Frontend

# 2. Install dependencies
npm install
# or
pnpm install
```

---

## 🔐 Environment Variables

Create a `.env.local` file in the root of the project:

```env
# ─── Backend API ──────────────────────────────────────────────────────────────
# URL of the Xiomara backend REST API
NEXT_PUBLIC_API_URL=http://localhost:8888

# ─── Next.js ──────────────────────────────────────────────────────────────────
# Optional: set to 'production' for secure cookies in deployment
NODE_ENV=development
```

> The backend URL is the only required environment variable. All other configuration is handled at the application level.

---

### Running the App

```bash
# Development (with Turbopack — fast refresh)
npm run dev

# Production build
npm run build
npm run start

# Lint
npm run lint
```

Open [http://localhost:3000](http://localhost:3000). You will be redirected to `/es` (the default locale) and then to `/es/auth/login` if not authenticated.

---

## 🔬 Core Modules

### Authentication

The auth flow is fully handled through **Next.js Server Actions** in `actions/auth.ts`. The login action calls the backend, receives a JWT, and stores it as a **secure, httpOnly cookie** (30-day expiry). All subsequent Server Action calls extract this token to authenticate with the backend API.

New users who sign up are placed in a **pending approval state** and redirected to `/auth/pending` until an admin approves their account. The `AuthContext` exposes `user`, `isAuthenticated`, `isLoading`, `logout`, and `refetchUser` to all client components via React Context + TanStack Query.

---

### Client & Campaign Management

Clients and campaigns are modeled as **folder entities** on the backend. When a client is created, a folder is created via `createClientAction()`. Campaigns are sub-folders nested under their client.

All data for a given client or campaign is scoped to its `folderId`. The selected client and campaign are persisted in cookies via `ClientContext` and `lib/dataPersistence.ts`, so the user's context survives page refreshes.

---

### Content Engine (AI Pipeline)

The Content Engine is a three-step AI workflow:

```
Step 1 — Fuentes (Sources)
  └── User selects one or more ingested sources from the folder

Step 2 — Chat / Summary
  └── AI generates a structured summary from the selected sources
  └── User can iterate, refine, or edit the summary
  └── Previous summaries are accessible via the Summaries dialog

Step 3 — Output
  └── User selects a prompt template
  └── AI generates a publication-ready output (social post, article, etc.)
  └── User can edit the output inline with the rich text editor
  └── Outputs are stored and viewable in the Output Card
```

All steps are folder-scoped — running the engine inside a campaign uses campaign-level sources, while running it at the client level uses client-level sources.

---

### Fuentes (Sources)

Sources are the raw input material for the AI engine. Users can ingest content from:
- **URLs** — web articles and pages
- **Documents** — uploaded files
- **Other source types** — via the drawer form with tabs (`SourcesDrawerForm`)

Sources are listed in paginated tables with search, and can be linked to or removed from folders.

---

### Knowledge Base

The knowledge base stores curated reference documents that provide persistent background context to the AI during content generation. Knowledge items are scoped per client and per campaign.

---

### Corresponsables & Telegram Integration

Corresponsables are team members or automated agents co-responsible for a client or campaign. The platform supports **Telegram bot listeners** configured via a token dialog (`TelegramTokenDialog`), which creates a listener on the backend that can ingest messages from Telegram into the sources pipeline.

---

### Templates

Templates are prompt configurations that drive the AI output step. They can be:
- **Global** — available to all users across the platform
- **User-specific** — private to the creating user

Templates are managed through `TemplatesContext`, which fetches and provides the list globally so the Content Engine and other components can access them without additional fetches.

---

## 🌐 Routing & i18n

Xiomara uses **next-intl** for full internationalization with locale-prefixed URLs.

| Locale | Prefix | Status |
|:---|:---|:---:|
| Spanish | `/es/...` | Default |
| English | `/en/...` | Supported |

**Route examples:**

```
/es/clients                                          → Client list (Spanish)
/en/clients                                          → Client list (English)
/es/clients/:clientId                                → Client dashboard
/es/clients/:clientId/campaigns/:campaignId          → Campaign dashboard
/es/clients/:clientId/campaigns/:campaignId/content-engine  → Content Engine
/es/clients/:clientId/knowledge                      → Knowledge base
/es/auth/login                                       → Login page
```

The **middleware** (`middleware.ts`) handles three concerns simultaneously:
1. **Locale routing** via `next-intl` middleware (detects locale from URL or browser preference)
2. **Auth guard** — unauthenticated users accessing protected routes are redirected to `/auth/login`
3. **Client selection guard** — users accessing the Content Engine without a selected client are redirected to `/clients`

All route strings are centralized in `lib/routes.ts` and helper functions (`getLocalizedRoute`, `getLocalizedRouteFromPathname`) ensure consistent locale-prefixed navigation throughout the codebase.

---

## 🎨 UI & Design System

The UI is built on **shadcn/ui** + **Radix UI** primitives styled with **Tailwind CSS v4**.

**Component highlights:**

| Component | Description |
|:---|:---|
| `metric-card.tsx` | KPI cards shown in the campaign metrics row |
| `rich-text-editor.tsx` | Quill-based editor for content creation and output editing |
| `media-post.tsx` | Preview component for formatted social media posts |
| `source-form-tabs.tsx` | Tabbed form for ingesting different source types |
| `url-input.tsx` | Specialized input for URL validation and entry |
| `file-upload.tsx` | Drag-and-drop file upload with preview |
| `ShadcnRowActions.tsx` | Standardized row action dropdown for all data tables |
| `delete-confirmation-dialog.tsx` | Reusable destructive action confirmation modal |

**Skeleton loading** — every auth form has a dedicated skeleton component (`skeletons/`) displayed via `Suspense` while the form component loads, ensuring smooth initial renders.

---

## 🤝 Contributing

Contributions are welcome. To get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'feat: add my feature'`
4. Push to your branch: `git push origin feature/my-feature`
5. Open a Pull Request against `main`

Please follow the code conventions in `.cursor/rules/project.mdc`:
- **TypeScript everywhere** — prefer interfaces over types, avoid enums
- **Functional components only** — no class components
- **Server Components first** — minimize `use client`, `useEffect`, and `useState`
- **Descriptive variable names** — use auxiliary verbs (`isLoading`, `hasError`, `canSubmit`)
- **Named exports** for all components
- **Lowercase with dashes** for directory names

---

## 📚 Resources

<p align="center">
  <a href="https://nextjs.org/docs">
    <img src="https://img.shields.io/badge/Next.js_Docs-black?style=for-the-badge&logo=next.js&logoColor=white"/>
  </a>
  <a href="https://next-intl-docs.vercel.app/">
    <img src="https://img.shields.io/badge/next--intl_Docs-A855F7?style=for-the-badge"/>
  </a>
  <a href="https://tanstack.com/query/latest">
    <img src="https://img.shields.io/badge/TanStack_Query_Docs-FF4154?style=for-the-badge&logo=reactquery&logoColor=white"/>
  </a>
  <a href="https://ui.shadcn.com/">
    <img src="https://img.shields.io/badge/shadcn%2Fui_Docs-18181B?style=for-the-badge&logo=shadcnui&logoColor=white"/>
  </a>
  <a href="https://zod.dev/">
    <img src="https://img.shields.io/badge/Zod_Docs-3E67B1?style=for-the-badge"/>
  </a>
</p>

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:F43F5E,40:EC4899,80:A855F7,100:6D28D9&height=120&section=footer&animation=fadeIn" width="100%"/>
</p>

<p align="center">
  Built by <a href="https://github.com/ahmadali507"><b>Ahmad Ali</b></a>
  <br/><br/>
  <a href="https://github.com/ahmadali507/Xiomara-Frontend">
    <img src="https://img.shields.io/github/stars/ahmadali507/Xiomara-Frontend?style=social"/>
  </a>
  &nbsp;
  <a href="https://github.com/ahmadali507/Xiomara-Frontend/fork">
    <img src="https://img.shields.io/github/forks/ahmadali507/Xiomara-Frontend?style=social"/>
  </a>
</p>
