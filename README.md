# 🌍 SiagaBencanaBojonegoro

**SiagaBencanaBojonegoro** is a web application built with **Next.js** and **Tailwind CSS**, designed to support the _Sustainable Development Goals (SDGs)_, particularly in terms of **disaster monitoring and preparedness** in Bojonegoro Regency, East Java.

> This application features an interactive Web GIS, community disaster reports, and a statistics dashboard to help with data-driven emergency response.

---

## 🚀 Tech Stack

- **Next.js** (Pages Router, no `src/` folder)
- **Tailwind CSS** (via CDN injection)
- **Leaflet.js** + **OpenStreetMap** (for the interactive map)
- **Supabase** (for Google authentication & user management)
- **Google Cloud Console** (OAuth2.0)
- **Local CSV** (as dummy data)

---

## 📦 Key Features

### ✅ Home (`/`)
- Interactive map with **Leaflet.js**
- Markers for each **district (kecamatan) in Bojonegoro**
- Marker colors based on impact level (redder = more severe)
- Info popups: number of villages affected by **floods, earthquakes, landslides**

### ✅ Report a Disaster (`/laporkan`)
- Disaster report form (select district, disaster type, description, photo upload)
- Timestamp recorded automatically
- Dummy report list with statuses: `Menunggu`, `Terkonfirmasi`, `Hoax`

### ✅ Admin Dashboard (`/admin`)
- Dummy report statistics (total reports, statuses)
- Report management table (edit, change status, delete)

---

## 🔐 Admin Access
Access to the `/admin` page is restricted to the email defined in `.env`:

```env
NEXT_PUBLIC_ADMIN_EMAIL=youremail@example.com
````

---

## 🔧 Project Structure

```
/pages
  /index.js
  /laporkan.js
  /admin.js
  /auth/callback.js
  /api
    /...
/components
/data
/public
```

---

## ⚙️ Local Installation

```bash
git clone https://github.com/romiwebdev/SiagaBencanaProjectSDGs.git
cd SiagaBencanaProjectSDGs
npm install
npm run dev
```

Add a `.env.local` file:

```env
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
NEXT_PUBLIC_ADMIN_EMAIL=rominmuh230@gmail.com
NEXT_PUBLIC_SUPABASE_REDIRECT=http://localhost:3000/auth/callback
```

---

## 🌐 Deployment

1. **Push to GitHub**
2. **Connect to [Vercel](https://vercel.com/)**
3. **Set the environment variables in Vercel according to `.env.local`**

---

## 🗺️ SEO & Sitemap

* Full favicon set (all sizes) is available in `/public`
* Sitemap and robots.txt are generated automatically
* SEO-friendly meta tags on all main pages

---

## ✅ Supported SDG Goals

* **Goal 11: Sustainable Cities and Communities**
* **Goal 13: Climate Action**

---

## 📌 Focused Area

**Bojonegoro Regency, East Java – Indonesia**

---

## 📄 License

MIT License © 2025 - romiwebdev

---

## 📣 Contributing

Pull requests are welcome! Feel free to fork this repo and submit a PR if you'd like to help develop further features.

<!-- last-updated -->
_Last updated: 2026-09-05_

