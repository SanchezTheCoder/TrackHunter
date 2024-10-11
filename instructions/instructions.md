# Project Overview
TrackHunter is a web-based SaaS tool designed to make track discovery from DJ sets on YouTube quick and seamless. Users simply input a YouTube link to a DJ set, and TrackHunter automatically extracts tracklists, organizing them in a user-friendly format. This tool saves DJs and music enthusiasts time by eliminating manual track identification and playlist creation.

Built with Next.js 14, Shadcn, tailwind, and Lucid icon for a modern, responsive UI.

# Core Functionalites
1. Tracklist Scraper: Scrapes the comments or description section of YouTube DJ sets to extract tracklists.
    1. User inserts the YouTube URL into the input field.
    2. User clicks the "Discover Tracks" button.
    3. The app makes an API request to the YouTube Data API v3 to fetch video details and comments.
    4. The app scrapes the YouTube video’s description and comments to extract the tracklist.
2. Unreleased Track Handling: Adds placeholders for tracks that are unreleased, so users can track them later.
    1. Identifies unreleased tracks marked as "ID" in the comments or description.
    2. Inserts placeholders for these tracks in the generated tracklist.
    Future plans include notifications when these tracks are officially released.
3. Neat Track Display: Presents a clean, organized list of tracks after scraping.
    1. Tracklist is displayed in a user-friendly format.
    2. Users can copy the tracklist or save it for future use.
4. Future Integrations:
    1.   Spotify Playlist Export: Planned feature to allow users to export the tracklist directly to Spotify.
    2. Track Release Notifications: Planned feature to notify users when unreleased tracks become available.

# Documentation
###

# Current File Structure
.
├── README.md
├── app
│   ├── favicon.ico
│   ├── fonts
│   ├── globals.css
│   ├── layout.tsx
│   └── page.tsx
├── components.json
├── instructions
│   └── instructions.md
├── lib
│   └── utils.ts
├── next-env.d.ts
├── next.config.mjs
├── package-lock.json
├── package.json
├── postcss.config.mjs
├── tailwind.config.ts
└── tsconfig.json
