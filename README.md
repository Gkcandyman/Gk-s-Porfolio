# Gowshik Karuneswaran G | Portfolio

Personal portfolio for an ERP and full stack developer. It is a plain static site with no build step.

## Files

- `index.html` the whole site (HTML, CSS and JavaScript)
- `img/` the photo and the chibi characters
- `api/ask.js` optional, lets the "Ask Gowshik" box answer with Claude (Vercel only)

## Put it live

**GitHub Pages (free, no setup)**
1. Upload all of these files to the root of this repo and commit to `main`.
2. Open Settings, then Pages. Under "Build and deployment" choose "Deploy from a branch", branch `main`, folder `/ (root)`, then Save.
3. After about a minute the site is at `https://gkcandyman.github.io/Gk-s-Porfolio/`.

**Vercel (same as the ERP)**
1. Import this repo in Vercel. Leave the framework as "Other" and the build command empty.
2. Deploy.

## Edit the content

Open `index.html` and search for the text you want to change. The answers for typed questions are in the `KB` list near the bottom of the file. The preset questions are in the `QA` list.

## Optional: Claude answers on Vercel

The typed-question box works without any setup, using the built-in answers. To let Claude answer instead:
1. Deploy on Vercel and add an environment variable `ANTHROPIC_API_KEY` in the project settings.
2. In `index.html` change `var USE_API = false;` to `var USE_API = true;`.
3. If the call ever fails, the site falls back to the built-in answers.
