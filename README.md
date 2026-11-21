# AL AHLY FC

A responsive, bilingual Arabic/English fan-app starter for following Al Ahly SC. The current version is a static, interactive frontend focused on clear source attribution and honest data availability: it does **not** invent match results, player statistics, news, or trophy totals.

## Run locally

Open `index.html` in a browser. No build step or package installation is required. The Google Fonts import is optional; the interface has fallback fonts.

## What works

- Responsive dark dashboard with Arabic RTL and English LTR layouts.
- Client-side section navigation for Home, Matches, Squad, News, and Honours.
- Language selection is remembered in local storage.
- Search input and keyboard shortcut (`/`); since no club dataset is connected, it explicitly reports that results are unavailable rather than fabricating matches.
- Links to the club's official website, schedule, results, and first-team pages.
- Empty/unavailable states where verified live information has not been integrated.

## Data and production status

This repository starts as an empty project. It currently has **no backend, database, authentication, admin dashboard, push notifications, licensed sports-data provider, or automated synchronization**. The official Al Ahly site is linked as the primary source, but this frontend does not scrape it or claim it has an API. Before publishing live data, add a server-side integration that is permitted by the source's terms, or use a licensed provider. Keep provider credentials on the server, store source URLs and retrieval timestamps with records, and show unavailable states when data cannot be verified.

Suggested production stack: Next.js or React frontend, a Node.js API, PostgreSQL/Supabase, and a licensed sports data API. Validate the official site's permitted integration methods and image/content rights before implementing ingestion.

## Official sources

- Arabic club website: https://www.alahlyegypt.com/ar
- Fixtures: https://www.alahlyegypt.com/en/football/schedule
- Results: https://www.alahlyegypt.com/en/football/results
- First team: https://www.alahlyegypt.com/en/football/first-team

## Branding

The shield in this starter is a decorative text mark, not the official club crest. Obtain permission and the correct asset before using official logos, player photography, or other protected content.
