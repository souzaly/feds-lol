<img width="1892" height="941" alt="hero" src="https://github.com/user-attachments/assets/336d92a3-da70-4be9-a036-167c6624dbff" />

<p align="center">
  <a href="https://feds.lol/">
    <h1 align="center">feds.cc</h1>
  </a>
</p>

<p align="center">
feds.cclol is a feature-rich link-in-bio tool with over 80,000 users.
</p>
<p align="center">
  <a href="https://www.linkedin.com/in/maria-nguyen-le">
    <img src="https://img.shields.io/badge/-MariaLe-blue?style=plastic-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/maria-nguyen-le/" alt="LinkedIn" />
  </a>
</p>
<br/>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#introduction">Intro</a>
    </li>
    <li>
      <a href="#techstack">Techstack</a>
    </li>
    <li><a href="#features-technical">Features</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
  </ol>
</details

<hr />

## Introduction

In this repository, you'll find **snippets of code** from my solo development and design of feds.lol.
Additionally, the `/images` folder contains **actual screenshots** of various pages, features and UI elements of the platform.
This repo doesn’t include full business logic or anything sensitive - just the core structure and my coding approach.

Further down, you can explore the **the nearly complete folder structure** of the project.

## Techstack

- nextjs 15 - framework
- typescript - language
- tailwindcss - css
- mysql - database
- drizzle - orm
- zustand - global state management
- zod - validation
- mailersend - emails
- stripe - payments
- vitest - tests

## Features

- server-side rendering (SSR)
- static site genetation (SSG)
- incremental static regeneration (ISR)
- react server components (RSC)
- streaming / partial loading (suspense + loading.tsx)
- dynamic routing with catch-all and optional segments
- nested layouts and parallel routes
- multi-tenancy e.g. maria.slat.cc
- file-based and dynamic metadata generation
- mutations via server actions
- tag-based revalidation (on-demand cache updates)
- login/register with discord oauth
- dynamic og:image generation (custom Open Graph API)
- webhooks for syncing external actions
- rich text editor
- 30+ advanced effects/animations created with css and framer-motion
- media proxy
- file uploading (images, audio, videos)
- integrated with spotify, discord, soundcloud, roblox, yt, twitch, steam, deezer, iconify-icons, github api
- reordering links, widgets, badges etc.
- promise-based toast system (auto cancel / status updates)
- analytics (top links, total and unique views, audience geo)
- admin dashboard for user management and editing articles
- state sync with zustand - instant live biolink preview feature
- analyze and visualize audio frequency - audio visualizer feature
- type-safe forms with zod + react-hook-form
- responsive modals – native drawers for mobile, dialogs on desktop
- partial use of shadcn/ui for consistent styling and accessible primitives

## Project Structure

```
  ├── app
  │   ├── (auth)
  │   ├── (errors)
  │   ├── (marketing)
  │   ├── [username]
  │   │   ├── page.tsx
  │   │   └── opengraph-image.tsx
  │   ├── api
  │   ├── casino
  │   ├── dashboard
  │   ├── docs.feds.lol
  │   │   └── [[...slug]]
  │   ├── error.tsx
  │   ├── not-found.tsx
  │   ├── providers.tsx
  │   ├── manifest.ts
  │   ├── robots.ts
  │   ├── sitemap.ts
  │   └── ...
  ├── components
  │   ├── dashboard
  │   ├── email
  │   ├── form
  │   ├── media
  │   ├── profile
  │   ├── shared
  │   └── ui
  ├── hooks
  ├── lib
  │   ├── analytics
  │   ├── api
  │   ├── auth
  │   ├── casino
  │   ├── constants
  │   ├── drizzle
  │   ├── features
  │   │   ├── accounts
  │   │   ├── actions
  │   │   ├── app
  │   │   ├── badges
  │   │   ├── comments
  │   │   ├── config
  │   │   │   ├── actions
  │   │   │   │   ├── assets.ts
  │   │   │   │   ├── avatar.ts
  │   │   │   │   ├── card.ts
  │   │   │   │   ├── colors.ts
  │   │   │   │   ├── comments.ts
  │   │   │   │   ├── fonts.ts
  │   │   │   │   ├── info.ts
  │   │   │   │   └── ...
  │   │   │   ├── queries.ts
  │   │   │   ├── defaults.ts
  │   │   │   ├── schemas.ts
  │   │   │   └── ...
  │   │   ├── embeds
  │   │   ├── giveaways
  │   │   ├── links
  │   │   ├── metadata
  │   │   ├── orders
  │   │   ├── profile
  │   │   ├── tags
  │   │   ├── templates
  │   │   ├── tracks
  │   │   ├── users
  │   │   │   ├── actions
  │   │   │   │   ├── email.ts
  │   │   │   │   ├── password.ts
  │   │   │   │   ├── username.ts
  │   │   │   │   ├── index.ts
  │   │   │   │   └── ...
  │   │   │   ├── utils
  │   │   │   │   ├── email.ts
  │   │   │   │   ├── user-id.ts
  │   │   │   │   ├── index.ts
  │   │   │   │   └── ...
  │   │   │   ├── validators
  │   │   │   │   ├── email.ts
  │   │   │   │   ├── username.ts
  │   │   │   │   ├── index.ts
  │   │   │   │   └── ...
  │   │   │   ├── queries.ts
  │   │   │   ├── roles.ts
  │   │   │   ├── schemas.ts
  │   │   │   └── types.ts
  │   │   └── ...
  │   ├── integrations
  │   ├── media
  │   ├── middleware
  │   ├── routes
  │   ├── server
  │   ├── stores
  │   ├── utils
  │   ├── zod
  │   ├── config.ts
  │   ├── email.ts
  │   ├── stripe.ts
  │   ├── types.ts
  │   ├── webhook.ts
  │   └── ...
  ├── styles
  ├── public
  ├── tests/casino
  └── ...
```

### Showcase (old)

Small showcase of some features such as tilting card, audio visualizer and thunder effect.

https://github.com/user-attachments/assets/250a19aa-0b7a-48ed-9dfb-a129b6cf737f

### Hero (old)

![image](https://github.com/user-attachments/assets/22fbdb42-f2cb-4324-8d61-39435530997d)
