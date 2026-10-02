# Savings Hub — Cloudflare Pages

Production files live in `/public`.

## Cloudflare Pages settings

Framework preset: None
Build command: leave blank
Build output directory: public
Root directory: leave blank
Production branch: main

Every push to `main` will deploy automatically.

## Updating the site

Replace the relevant files inside `/public`, then:

    git add .
    git commit -m "Update Savings Hub"
    git push

Cloudflare Pages will build/deploy automatically.

## Supabase

The website continues to use the existing Supabase project.
The `savings-shop` Edge Function stays in Supabase — it does NOT move to Cloudflare.

If you later add OAuth or magic-link authentication, add the new Cloudflare Pages
domain/custom domain to the Supabase Auth redirect URL allow-list.

## Current release

RC5.3.1:
- polished website
- Savings Shop
- Bank Switch Shop beta
- account intelligence/history
- graph scroll-position bug fixed
- V5.0.1 first-login cloud safety retained
