# Southern Africa After Sunset — GitHub Pages Website

A static, public-safe GitHub Pages site for a personal family-facing trip announcement page.

## What this site is

This is a luxury travel magazine-style preview page for the personal trip **Southern Africa After Sunset**.

It combines:

- Countdown announcement
- Interactive route showcase
- Family-friendly destination highlights
- Safari and Cape Town sections
- Photo placeholders
- Playlist mood section
- Privacy note

## What this site is not

This is not a business website, booking engine, dashboard, travel agency system, or private planning file.

Do not publish private logistics here.

## File structure

```text
.
├── index.html
├── 404.html
├── .nojekyll
├── assets
│   ├── css
│   │   └── styles.css
│   └── js
│       └── main.js
└── data
    └── trip.json
```

## How to edit trip content

Most public trip content lives in:

```text
data/trip.json
```

Edit this file to update:

- Trip title
- General dates
- Countries
- Route order
- Backup route
- Airport strategy summary
- Public-safe home base areas
- Destination highlights
- Photo placeholder labels
- Playlist mood
- Privacy rules

## How to add photos

The gallery currently uses placeholders that say:

> Replace with your photo.

To add real photos later, create an image folder such as:

```text
assets/img/
```

Then update `index.html`, `styles.css`, or `main.js` depending on how you want to display them.

Only use family-safe photos on this public site.

## Privacy rules

Do not include:

- Adult/private nightlife details
- Exact flight numbers
- Room numbers
- Confirmation numbers
- Cash buffer
- Emergency plan
- Passport details
- Private contacts
- Payment details
- Exact live logistics

The site intentionally says:

> Some details are kept private for safety.

## Deploy to GitHub Pages

1. Create a new GitHub repository.
2. Upload all files and folders from this project.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/root` folder.
6. Save.
7. GitHub will publish the site at your GitHub Pages URL.

## Local preview

Because the site loads `data/trip.json`, previewing with a simple local server works better than opening `index.html` directly.

From the project folder, run:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

No backend, paid API, login, build tools, or external dependencies are required.
