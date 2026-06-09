# HAIC Website

## What This Is
Static site for the **Human AI Consortium** — a credibility/legitimacy site for potential clients.
Five pages: Home, About, Members, Services, Contact.

## Tech
Plain HTML/CSS/JS. No framework, no build step, no CMS.
Hostable on GitHub Pages, Netlify, or Cloudflare Pages (free tier).

## File Structure
```
index.html        Home
about.html        About HAIC
members.html      Our Members
services.html     Services
contact.html      Contact
css/style.css     All styles (CSS variables at top)
js/nav.js         Mobile hamburger toggle only
assets/images/    Member headshots (empty at launch — using initials avatars)
```

## Visual Identity
- **Navy** `#1C3F6E` — nav, headings, CTA bars (matches charter PDF)
- **Blue** `#2563A8` — links, section labels, accent borders
- **Font** — Inter via Google Fonts
- **Layout** — 1100px max-width, fixed top nav, text-forward (no hero images)

## Key Content Sources
- `claude.md.txt` — original planning brief
- `HAIC-Member-Charter-Apr2026.docx` — core beliefs, operating norms, member list
- `Strategic_Vision_Working_Draft.docx` — mission, methodology (Structured Disruption), OI framework, client profile
- `AI & Agility Team Contact Info.xlsx` — all 11 member names, emails, LinkedIn URLs

## Members (11 total)
Aaron Libby, Andrew Gore, Cameo Doran, David Posey, Dean Kynaston,
Eliza Moody, Masa Maeda, Michael Moore, Nate Jones, Reed Shell, Steve Ostermiller

Contact currently routes to Steve Ostermiller (sostermiller@gmail.com) via mailto.

## Adding Member Headshots
Replace the `.member-avatar` div in `members.html` with:
```html
<img src="assets/images/firstname-lastname.jpg" alt="Member Name" class="member-avatar">
```
Add to CSS: `.member-avatar img { width: 72px; height: 72px; border-radius: 50%; object-fit: cover; }`
