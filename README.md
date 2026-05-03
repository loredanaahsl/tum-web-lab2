# Biskuit — Lab 4: Static Site Generator & Git-based CMS

## 1. Project Overview
This project represents the migration of a static landing page into a modern architecture based on a Static Site Generator (SSG) and a Git-based Content Management System (CMS).

The goal was to improve maintainability, scalability, and allow non-technical users to edit content without modifying source code.

---

## 2. Technologies Used

- **Astro** — Static Site Generator (SSG)
- **Netlify** — Hosting and deployment platform
- **Decap CMS** — Git-based CMS
- **GitHub** — Version control system

---

## 3. Key Features

- Fully responsive landing page
- Modular structure using Astro components
- Dynamic content loaded from JSON files
- Content editable through a CMS interface
- Automatic deployment after each content update

---

## 4. Content Management

All editable content is stored in:

- `src/data/site.json` — general site content (hero, about, contact, etc.)
- `src/data/cookies.json` — product data (weekly and classic cookies)

Using Decap CMS, content editors can:
- modify text (titles, descriptions)
- update prices
- change images
- add or remove items

Each change creates a commit in the GitHub repository and triggers automatic redeployment.

---

## 5. Deployment

The project is deployed using Netlify.

- **Live website:**  
  https://spontaneous-daifuku-905522.netlify.app/

- **CMS panel:**  
  https://spontaneous-daifuku-905522.netlify.app/admin/

---

## 6. How It Works

1. The site is generated statically using Astro
2. Content is stored in JSON files
3. Decap CMS provides a UI for editing content
4. Changes are committed to GitHub automatically
5. Netlify detects changes and rebuilds the site

---

## 7. Running Locally

```bash
npm install
npm run dev