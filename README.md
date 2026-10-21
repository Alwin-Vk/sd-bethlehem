# SD’s BETHLEHEM

A standalone housewarming invitation for Sherin & Dibiya, hosted at **https://sd-bethlehem.com**.

- **When:** Saturday 7 November 2026, from 6:00 PM
- **Where:** 42 Carrs Peninsula Road, Junction Hill, NSW, Australia
- **Site:** `index.html` with assets in `assets/bethlehem/`
- **Hosting:** GitHub Pages, branch `main`, folder `/(root)`. The `CNAME` file contains `sd-bethlehem.com`.
- **Backend:** Independent Google Apps Script for private RSVP submissions and public, immediately visible wishes. See `google-apps-script.js` for its source; the web app is deployed separately and the endpoint is already configured in `index.html`.
- **Privacy:** The Google Sheet should remain private. Guest-submitted wishes are public on the invitation.
- **Important:** The wedding website and its separate repo `Alwin-Vk/wedding-invite` must not be modified for this site.

## Connect the domain

1. In this repo's **Settings → Pages**, set **Deploy from a branch**, select `main` and `/(root)`, then save.
2. In Hosting Ireland DNS for `sd-bethlehem.com`, add apex A records pointing to `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, and `185.199.111.153`.
3. Optional `www` alias: create CNAME record `www` → `Alwin-Vk.github.io`. Remove only conflicting `www` records.
4. In **Settings → Pages**, confirm the custom domain `sd-bethlehem.com`, wait for DNS verification and enable **Enforce HTTPS**.
5. Test the hero, all 10 story photos, music, RSVP, public wishes and Google Maps from a private browser window.

Do not enable DNS forwarding / masking or replace the original wedding repo's `CNAME`. DNS changes affect only `sd-bethlehem.com`.

## Source

Migrated from `Alwin-Vk/wedding-invite/engagement/` at 961cd2eaedaf3f958b5eefa5a80d0897cc588c33. Assets are copied at their original Git blob SHAs; no wedding homepage files are included.
