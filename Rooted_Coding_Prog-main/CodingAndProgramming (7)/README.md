# 2026 FBLA Coding and Programming Challenge
# Rooted

A web application what allows users to discover and support local businesses. Users can browse businesses, leave reviews, save favorites, and business owners can manage their listings and deals.

Built for the 2026 FBLA Coding and Programming Challenge

---

## Overview

Rooted connects community members with loca l businesses through an interactive platform featuring:

- **Business Discovery** - Browse, search, and filter local businesses with an interactive map
- **User Accounts** - Secure authentication with personalized favorites and review history
- **Review System** - Rate and review businesses with 1-5 star ratings
- **Business Management** - Owners can create, edit, and manage their business listings
- **Deals & Promotions** - Business owners can post special offers
- **Accessibility** - Screen Reader Accessible & full keyboard navigation

---

## Tech Stack

**Frontend**
- React 18.3.1 + TypeScript
- Tailwind CSS 4.1.12
- Vite 6.3.5
- Radix UI + shadcn/ui components

**Backend**
- Supabase (PostgreSQL database)
- Supabase Auth (user authentication)
- Supabase Storage (image uploads)
- PostgREST (auto-generated REST API)
- Deno + Hono (edge functions)

---

## Getting Started

### Prerequisites

- Node.js v18.0.0+
- npm or pnpm
- Supabase account 

### Installation

1. **Clone and install**

```bash
git clone https://github.com/yourusername/rooted.git
cd rooted
npm install
```

2. **Set up Supabase**

- Create a new project at [supabase.com](https://supabase.com)
- Note your Project URL, Anon Key, and Service Role Key

3. **Configure secrets**

The app will prompt you for Supabase credentials on first run:
- `SUPABASE_URL`
- `SUPABASE_ANON_KEY`
- `SUPABASE_SERVICE_ROLE_KEY`

4. **Run the app**

```bash
npm run dev
```

App will be available at `http://localhost:5173`

---

## Running the Application

### Development

```bash
npm run dev          # Start dev server with hot reload
```

### Production

```bash
npm run build       
npm run preview      # Preview production build locally
```

### Development Workflow

1. Start dev server with `npm run dev`
2. Build for production with `npm run build`

---

## Project Structure

```
rooted/
├── src/
│   ├── app/
│   │   ├── components/       # react stuff
│   │   ├── services/         # api and auth logic
│   │   │   ├── authService.ts
│   │   │   └── dataService.ts
│   │   ├── types/            # typescript interface
│   │   └── App.tsx           # root component
│   └── styles/               # styles and theme
├── supabase/functions/server/ # backend logic and migrations
├── package.json
└── vite.config.ts
```

## Key Features

### For Users

**Browse & Discover**
- View all businesses on Browse page or interactive map
- Filter by category (Restaurant, Cafe, Retail, Service, Health, Entertainment)
- Filter by price range and rating
- Search by business name
- Sort by rating, price, name, or newest

**Reviews & Ratings**
- Leave 1-5 star reviews with text comments
- Edit or delete your own reviews
- View all reviews for each business
- Average ratings displayed on business cards

**Favorites**
- Save businesses to your favorites list
- Quick access to favorite businesses
- Persistent across sessions

### For Business Owners

**Business Management**
- Create new business listings
- Upload business images (drag-and-drop)
- Edit business details (name, description, category, price, contact)
- Delete businesses

**Deals & Promotions**
- Create time-limited deals
- Set expiration dates
- Edit or delete deals
- Deals displayed on business detail pages


---


## Project Statistics

- **Files**: 73 TypeScript/CSS files
- **Components**: 65 (18 custom + 47 shadcn/ui)
- **Dependencies**: 54 npm packages
- **Database Tables**: 6 tables
- **API Endpoints**: 15+ REST endpoints

---

## License

MIT License - Copyright (c) 2026 Rooted

---

## Credits

Built with React, TypeScript, Tailwind CSS, and Supabase. UI components from shadcn/ui and Radix UI. Icons from Lucide. 


---
