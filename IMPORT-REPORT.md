# Import report: David Nichol MD

Imported from https://davidnicholmd.com (Squarespace 7.0) on 2026-11-03 with `openspace import squarespace`.
Sources: page HTML and the sitemap, Squarespace's `?format=json` data (owner mode). 47 requests.

## Summary

- **11** pages, **8** collection items in 1 collection(s)
- **10** media files (3.9 MB) downloaded into `media/`
- **9** redirects so old addresses keep working
- **4** item(s) need your attention (below)

## Pages

| Squarespace | OpenSpace | Title | Sections | Blocks |
| --- | --- | --- | ---: | ---: |
| `/` | `/` | David Nichol MD \| Home | 2 | 6 |
| `/david-nichol-md` | `/david-nichol-md` | About Me | 2 | 4 |
| `/treatment/options` | `/treatment/options` | Options | 2 | 6 |
| `/treatment/emdr` | `/treatment/emdr` | EMDR | 2 | 2 |
| `/treatment/brainspotting` | `/treatment/brainspotting` | Brainspotting | 2 | 2 |
| `/health-information` | `/health-information` | Health Information | 4 | 6 |
| `/mental-health-information` | `/mental-health-information` | Mental Health Information | 4 | 6 |
| `/links` | `/links` | Links | 1 | 1 |
| `/studies` | `/studies` | Studies | 1 | 3 |
| `/recommended-books` | `/recommended-books` | Recommended Books | 1 | 1 |
| `/contact` | `/contact` | Contact | 2 | 3 |

## Collections

| Squarespace | OpenSpace | Kind | Items | Drafts |
| --- | --- | --- | ---: | ---: |
| `/blog` | `/blog/` | blog | 8 | 0 |

## Design

The look was recreated with OpenSpace's own design system (Site Styles tokens, section color themes, layouts and section presets), not by copying Squarespace's template CSS or code.

- The Squarespace palette has no strong color (none found), so the Monochrome palette is used.
- Fonts on Squarespace: adobe-garamond-pro → pairing "Fraunces & Hanken Grotesk" (Fraunces / Hanken Grotesk), the closest curated match. Licensed fonts can be uploaded in Site Styles → Fonts.
- Type scale on Squarespace: Heading 1 is 1.8× body text. Density "airy" from the section heights.
- adobe-garamond-pro (licensed from Adobe Fonts) can't be copied, so EB Garamond — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- proxima-nova (licensed from Adobe Fonts) can't be copied, so Sofia Sans — the closest measured shape (x-height, width) among free fonts — stands in. With a web licence, upload the real font in Site Styles → Your fonts.
- Type scale on Squarespace (the live site, measured in a browser) kept: display 59px caps, heading 1 32px/30px caps, body 18px/18px.
- Page rhythm on Squarespace (the live site, measured in a browser): sections padded 127px (26px on phones) — kept in Site Styles.

Design check: 0 error(s), 16 warning(s).

- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/): “Explore Now →” jumps from Heading 1 to Heading 3, skipping a level.
- warning (/): “David Nichol MD | Home” has no clear call to action — nothing tells visitors what to do next.
- warning (/david-nichol-md): An image in this image block has no alt text, so people using screen readers won't know what it shows.
- warning (/david-nichol-md): “About Me” has no clear call to action — nothing tells visitors what to do next.
- warning (/treatment/options): “Conditions I work with” is a second Heading 1 on this page. Use one Heading 1 per page.
- warning (/treatment/options): “Online psychological tests” is a second Heading 1 on this page. Use one Heading 1 per page.
- warning (/treatment/options): “Options” has no clear call to action — nothing tells visitors what to do next.
- warning (/treatment/emdr): “EMDR” has no clear call to action — nothing tells visitors what to do next.
- warning (/treatment/brainspotting): “Brainspotting” has no clear call to action — nothing tells visitors what to do next.
- warning (/health-information): “Health Information” has no clear call to action — nothing tells visitors what to do next.
- … and 4 more: run Design check in Studio or `design_check` with Claude.

## Needs attention

### Custom code and embeds

- Site-wide Code Injection was found (1 snippet(s)). It was **not** copied: review it and add what you still need in Settings → Advanced (head/footer code). Squarespace-specific scripts won't work here. _(site)_

### Forms and newsletter

- Form "Contact Form" recreated with 3 field(s). Submissions now arrive in the OpenSpace inbox; Squarespace form integrations (Google Drive, Mailchimp, Zapier…) need setting up again. _(/contact)_

### Links

- Link to /options led to a page that wasn't imported; it now points at the home page. Point it at the right page. _(/)_
- Text link to /options led to a page that wasn't imported; the link was removed. _(/)_

### Design

- A photo section's overlay was darkened from 30% to 70% so its text stays readable. _(/)_
- A photo section's overlay was darkened from 30% to 45% so its text stays readable. _(/david-nichol-md, /treatment/options, /treatment/emdr, /treatment/brainspotting, +1 more)_

### Other

- The page had no Heading 1; its first heading was made the Heading 1 (search engines and screen readers use it). _(/contact)_

## Redirects

Saved in `content/site.json` (`redirects`), published with the site:

| From | To |
| --- | --- |
| `/blog/2021/6/26/treating-ptsd-a-review-of-evidence-based-psychotherapy-interventions` | `/blog/treating-ptsd-a-review-of-evidence-based-psychotherapy-interventions/` |
| `/blog/2021/6/24/a-history-of-the-pharmacologic-treatment-of-bipolar-disorder` | `/blog/a-history-of-the-pharmacologic-treatment-of-bipolar-disorder/` |
| `/blog/2021/6/24/tms-transcranial-magnetic-stimulation-for-depression` | `/blog/tms-transcranial-magnetic-stimulation-for-depression/` |
| `/blog/2021/6/24/pharmacological-treatment-of-depression-international-review` | `/blog/pharmacological-treatment-of-depression-international-review/` |
| `/blog/2021/6/24/treatment-of-anxiety` | `/blog/treatment-of-anxiety/` |
| `/blog/2020/8/21/ketamine-assisted-psychotherapy` | `/blog/ketamine-assisted-psychotherapy/` |
| `/blog/2020/8/21/sleep-tips` | `/blog/sleep-tips/` |
| `/blog/2020/8/21/a-poem` | `/blog/a-poem/` |
| `/home` | `/` |

## Not moved by the importer

- Orders, customers, inventory, discounts, gift cards, shipping and tax settings (commerce stays in Squarespace until you switch).
- Newsletter subscribers, form submissions, member accounts and blog comments.
- Scheduling (Acuity), donations, digital-download files and anything behind a login.
- Squarespace analytics and SEO history (search engines follow the redirects).

## Next steps

1. `npm install`, then `npx openspace check` (it should report no errors) and `npx openspace dev` to look around.
2. Bring it to visual parity with Claude: in this folder run `claude`, then `/openspace:import-squarespace` (or ask Claude to compare each page with the original). It screenshots both sites at desktop and mobile and adjusts presets, Site Styles and sections — never raw HTML.
3. Fix the items under **Needs attention**, then publish (push to GitHub, or `publish` with Claude).
4. Move the domain only after the new site is live and checked:
   - add the custom domain in OpenSpace (`deploy.customDomain` in `openspace.json`, or the Hub);
   - at your DNS provider (Squarespace Domains or elsewhere), point the records at the new host as the domain guide says (GitHub Pages: `A`/`CNAME` records; Cloudflare: the Pages project's records);
   - keep the Squarespace subscription until the new site serves your domain over HTTPS and the redirects work; then cancel it (and transfer the domain away from Squarespace if you like).

