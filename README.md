# Manifest.AI — Full Stack AI App Builder

Manifest.AI is a full-stack AI-powered app builder built from scratch using Next.js, Supabase, Gemini AI, Cline SDK, Sandpack, Prisma, Clerk, and Shadcn UI.

It allows users to describe an app idea in natural language, upload reference images, and generate working React applications with live code and browser preview.

---

## Overview

Manifest.AI turns a simple prompt into a working React project.

Users can create new workspaces, chat with AI, generate code, preview the app instantly, upload reference images, and improve the project using an AI-powered file-by-file workflow.

The platform is designed as a modern app-generation workspace with persistent projects, credit-based usage, image uploads, live preview, and an autonomous improvement agent.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js 15, App Router, TypeScript |
| Authentication | Clerk |
| Billing | Clerk Billing |
| Database | Supabase Postgres |
| ORM | Prisma |
| Image Storage | Supabase Storage |
| AI Model | Gemini Flash |
| AI Agent | Cline SDK |
| Code Preview | Sandpack |
| Rate Limiting | Arcjet |
| UI | Shadcn UI |
| Styling | Tailwind CSS v4 |

---

## Core Features

### Landing Page

- Premium dark landing page
- Animated AI-style background
- Prompt textarea for app ideas
- Suggestion chips for quick prompts
- Browser preview mockup
- Features, workflow, pricing, and CTA sections

### Authentication & Billing

- Clerk authentication
- Google OAuth login
- User sync with Supabase
- Free, Starter, and Pro plans
- Credit-based usage system
- Plan detection using Clerk billing

### Workspace

- Split layout with Chat, Code, and Preview panels
- Persistent workspace history
- AI chat with markdown rendering
- Streaming-style assistant messages
- Image upload through Supabase Storage
- User avatars and auto-scroll chat UI

### AI Code Generation

- Gemini-powered React app generation
- API route: `/api/gen-ai-code`
- Generates structured JSON output:

```json
{
  "assistantMessage": "",
  "title": "",
  "files": {},
  "dependencies": {}
}
