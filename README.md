# Where Is My Bus

Where Is My Bus is a React web app concept for exploring public transport in Bidar, Karnataka. It provides screens for a live bus map, routes, stops, and individual bus tracking, with a responsive navigation layout.

> **Project status:** The current repository is a frontend prototype. Its bus and route information is sample data; live GPS tracking, ETA services, and user authentication require backend integrations that are not included here.

## Features

- Bidar Transit welcome and sign-in style screen
- Map, routes, stop details, and bus tracking views
- Responsive bottom navigation for map, routes, alerts, and saved items
- Sample bus, route, and stop data in `src/constants.ts`
- React, TypeScript, Vite, Tailwind CSS, and Leaflet dependencies

## Requirements

- Node.js 20 or later
- npm

## Run locally

```bash
npm install
npm run dev
```

Vite starts the development server on port `3000`. Use the URL printed in the terminal.

## Available scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server on port 3000 |
| `npm run build` | Create a production build in `dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run lint` | Run the TypeScript compiler without emitting files |

## Environment variables

Copy `.env.example` to `.env.local` if you are configuring integrations:

```env
GOOGLE_MAPS_PLATFORM_KEY=
GEMINI_API_KEY=
```

Keep real keys private. The current screens use sample app data, and configuring these values alone does not connect live bus tracking or authentication.

## Project structure

```text
src/
  components/   Shared navigation components
  screens/      Login, map, routes, stop, and tracking screens
  App.tsx       App layout and routes
  constants.ts  Sample buses, routes, stops, and image URLs
  index.css     Global styles
  main.tsx      React entry point
```

## Notes

- The login screen is a presentation flow and does not authenticate users.
- Alerts and saved pages currently show placeholder content.
- Replace sample data and connect trusted backend services before relying on the app for real-time transit information.
