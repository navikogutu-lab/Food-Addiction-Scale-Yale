# Deploy Instructions

All commands run from this folder: `c:\Navick\Yale Food Addiction Scale\`

---

## Step 1 — Install GitHub CLI (if not already)
```
winget install GitHub.cli
```
Then authenticate:
```
gh auth login
```
Choose: GitHub.com → HTTPS → Login with browser

---

## Step 2 — Create private GitHub repo & push

```bash
gh repo create yale-food-addiction-scale --private --source=. --remote=origin --push
```

That single command creates the private repo, sets origin, and pushes.

---

## Step 3 — Deploy live URL via Vercel

```bash
npx vercel login
npx vercel --prod
```

- When prompted for project settings, accept all defaults
- Vercel will output a live URL like: `https://yale-food-addiction-scale-xxx.vercel.app`

---

## Step 4 — Embed anywhere with this iframe

Replace `YOUR_VERCEL_URL` with the URL from Step 3:

```html
<iframe
  src="YOUR_VERCEL_URL"
  title="Yale Food Addiction Scale 2.0 | Discover Health Group"
  width="100%"
  height="900"
  style="border:none; border-radius:12px; overflow:hidden;"
  loading="lazy"
  allow="clipboard-write"
></iframe>
```

---

## Quick one-liner (after gh auth login + vercel login)

```bash
gh repo create yale-food-addiction-scale --private --source=. --remote=origin --push && npx vercel --prod
```
