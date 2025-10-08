# Resume App — Vercel Ready

One-folder Next.js app with Stripe checkout and a simple resume builder.

## Quick Deploy (Vercel)

1) Create a new GitHub repo. Upload all files.
2) In Vercel: **New Project** → Import the repo.
3) Set **Environment Variables**:
   - `NEXT_PUBLIC_URL` = your site URL (e.g. https://your-app.vercel.app)
   - `STRIPE_SECRET_KEY` = your Stripe secret key
   - Optional: `STRIPE_WEBHOOK_SECRET` when webhooks are set up
4) Framework Preset: **Next.js**. Root directory: `/`.
5) Deploy. Visit `/pricing` to test checkout.

## Local Dev

```bash
pnpm i # or npm i
pnpm dev # or npm run dev
```

## Stripe Prices

Update price IDs in `/app/pricing/page.tsx` or use env and read them in the API route.

## Notes

- Builder exports a `.txt` for simplicity. You can upgrade to a PDF export later.
- Webhooks route is a placeholder.
- Tailwind included via `app/globals.css`.
