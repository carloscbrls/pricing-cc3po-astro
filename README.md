# pricing.cc3po.com

Transparent pricing page for CC3PO services.

## Setup Complete ✓

- Astro project created at `/Users/cc3po/.openclaw/workspace/pricing-cc3po-astro`
- GitHub repo: https://github.com/carloscbrls/pricing-cc3po-astro
- Build: `npm run build`
- Output: `dist/`

## Netlify Deployment (Pending)

### Option 1: CLI (requires auth)
```bash
cd /Users/cc3po/.openclaw/workspace/pricing-cc3po-astro
netlify login
netlify deploy --prod --site-name=pricing-cc3po --dir=dist
```

### Option 2: GitHub + Netlify UI
1. Go to https://app.netlify.com
2. "Add new site" → "Import existing project"
3. Connect GitHub repo: `carloscbrls/pricing-cc3po-astro`
4. Build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
5. Set custom domain: `pricing.cc3po.com`

## DNS Configuration (after Netlify deployment)

At SiteGround DNS:
- Add CNAME record: `pricing` → `[netlify-subdomain].netlify.app`
- Or use Netlify DNS for automatic SSL

## Features

- 3 pricing tiers: Starter, Growth, Enterprise
- Add-on services section
- FAQ section with 6 questions
- Trust bar with stats
- CTA section linking to offers.cc3po.com/contact
- Dark theme matching CC3PO ecosystem
- Responsive design

## Pricing Values

All prices are placeholders. Update in `src/pages/index.astro`:
- Starter tier: One-time services ($299-$799)
- Growth tier: Monthly retainers ($199-$1,499/mo)
- Enterprise tier: Custom pricing
- Add-ons: $299-$599