# Utopia Fitness — Netlify Production Bundle

**Utopia Fitness** is a responsive fitness, GPS performance telemetry, and metabolic nutrition web application that combines the best of **Strava** (interactive GPS route & elevation scrubbing, live workout simulator, KOM/QOM segment leaderboards, Kudos club feed) and **MyFitnessPal** (bi-directional workout-to-calorie dynamic allowance, macro/micronutrient tracking, laser barcode scanner simulator, and meal diary), plus **Biometric Recovery & Anatomical Muscle Fatigue Mapping**.

## Folder Structure
- `index.html` — Complete, responsive single-page web application (works across 320px mobile, tablet, laptop, and 4K screens).
- `netlify.toml` — Zero-config Netlify edge headers, caching rules, and SPA routing configuration.
- `_redirects` — Netlify SPA fallback rules (`/* /index.html 200`).
- `manifest.json` — Progressive Web App (PWA) metadata.
- `robots.txt` — Search engine crawler configuration.

## How to Deploy to Netlify (3 Easy Ways)

### Method 1: Netlify Drop (Fastest — 10 Seconds)
1. Go to [app.netlify.com/drop](https://app.netlify.com/drop).
2. Drag and drop this entire unzipped folder (or `utopia-fitness-netlify.zip`) directly into the browser window.
3. Your site will be live on a global HTTPS Netlify CDN URL immediately!

### Method 2: Netlify CLI
```bash
npx netlify-cli deploy --dir=. --prod
```

### Method 3: Git Continuous Deployment
1. Push these files to a GitHub, GitLab, or Bitbucket repository.
2. In Netlify, click **Add new site → Import an existing project**.
3. Leave the build command blank and set the **Publish directory** to `.`.
