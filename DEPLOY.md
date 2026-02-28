# Yale Food Addiction Scale 2.0 — Deployment Reference

## ✅ Status: LIVE

| Item | Value |
|---|---|
| **Live URL** | https://yale-food-addiction-scale.vercel.app |
| **GitHub repo** | https://github.com/navikogutu-lab/Food-Addiction-Scale-Yale |
| **Vercel project** | navikogutu-labs-projects/yale-food-addiction-scale |
| **Deployed** | Vercel Production (Portland, US-West) |

---

## Embed Code

Copy `iframe-embed.html` or paste this anywhere on discoverhealthgroup.com:

```html
<iframe
  id="yfas-embed"
  src="https://yale-food-addiction-scale.vercel.app"
  title="Yale Food Addiction Scale 2.0 | Discover Health Group"
  width="100%"
  height="860"
  style="border:none; border-radius:12px; display:block;"
  loading="lazy"
  allow="clipboard-write"
></iframe>
```

---

## To redeploy after changes

```bash
cd "c:/Navick/Yale Food Addiction Scale"
git add index.html
git commit -m "your message"
git push origin master
vercel --prod
```
