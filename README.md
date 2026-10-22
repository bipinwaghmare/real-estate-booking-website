# Haven Estate — Real Estate Website Demo

A responsive multi-page real estate website built with HTML, CSS and vanilla JavaScript. Includes sample listings, a property gallery, a demo brochure PDF, a video sample, agent login, listing management, and an interactive floor/flat availability selector.

## Pages and features
- `index.html` — home page, featured properties and sample brochure link
- `properties.html` — searchable and filterable property listings
- `property.html?id=p1` — property details, photo gallery, video and interactive floor/flat selector
- `gallery.html` — clickable photo gallery and video tours
- `contact.html` — enquiry form (opens the visitor's email app)
- `login.html` — demo agent login
- `dashboard.html` — add/edit/delete listings, photos, videos, overall availability and individual flat statuses
- `assets/haven-estate-demo-brochure.pdf` — fictional sample property brochure

## Run locally
1. Extract this ZIP.
2. Open a terminal in the `real-estate-website` folder.
3. Run `python -m http.server 8000`.
4. Open `http://localhost:8000` in your browser.

### Demo login
- Email: `agent@havenestate.example`
- Password: `HavenDemo2026!`

## Demo content
Property names, availability, prices, contact information and brochure details are fictional placeholders. Property photos load from Unsplash and the sample video loads from Google's public sample-video bucket, so an internet connection is needed for those assets. Replace all sample material before publishing.

## Important: prototype, not production security
This is a front-end prototype. Login is checked in browser JavaScript, not by a secure server. Property listings, flat status, and uploaded media are stored in the current browser's `localStorage`; they do not sync across devices and may be cleared. Browser developer tools can bypass demo restrictions. Large photo/video uploads can exceed browser storage limits. The contact form opens the visitor's email app rather than sending enquiries to a server.

Before going live, connect a backend such as Supabase or Firebase with server-verified accounts, database access rules, cloud media storage, a real enquiry endpoint, HTTPS, and backups. Enforce permissions on the server, not just in the browser.
