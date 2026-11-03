# Visual fidelity

Overall match: **20/100** — fonts, type sizes, spacing and each section measured in a browser on both sites, and how alike the pages look as pictures, each counted from what two unrelated pages score (0) to identical (100); the weaker of the two counts double, and so do the weakest page and device. How it's scored: docs/qa/import-fidelity.md.

**Next step:** The automatic move is rough (20/100): the words and pictures came across, but most of the design didn't. That's normal for custom-built sites. Claude can make it match closely: in Claude with the OpenSpace connector, use the finish-a-move prompt (or Studio's "Finish it with Claude"). It compares the old and new pages side by side and rebuilds what didn't come across, keeping every word and picture editable.

Scored two ways, side by side: **20/100 corrected**, 20/100 by the strict v3 scorer. The corrected score reads three things the strict one gets wrong (navigation in a header themed "brand", off-screen slides counted as columns, a picture-only band on a phone); the pages below list where it did.

Before auto-tuning: 18/100. What it changed:

- h2: 22px, 22px on phones
- h3: 16px, 16px on phones, tracking 0em
- button: 18px, tracking 0.167em, uppercase
- h2: in the label font, as on the original
- h3: in the label font, as on the original
- content width 1400px
- section padding 200px

Recreating low-scoring sections as custom components didn't raise the score (20/100), so none were kept.

## / at 1440px — 0/100

Checks passed: 74% · screenshots 67% alike (two unrelated pages compare at about 55%) · 0% of its sections found.

Original: https://www.davidnicholmd.com/home/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Buttons: present | proxima-nova 18px | not found | **differs** |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Section padding | 127px | 100px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 0 | Present: DAVID NICHOL MD → no matching section |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).

## / at 390px — 40/100 (strict v3: 36/100)

Corrected scoring on this page:

- Section 2: columns counted on screen only (2 → 2 counted as 1 → 2; what's off screen or inside one slideshow or map isn't a column).
- Section 3 (a picture alone on a phone) is the picture of section 2, which holds it with its words.
- Section 5 (a picture alone on a phone) is the picture of section 2, which holds it with its words.

Checks passed: 75% · screenshots 76% alike (two unrelated pages compare at about 65%) · 83% of its sections found.

Original: https://www.davidnicholmd.com/home/  
Imported: / (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 26px | 15.5px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | (no heading) | 33 | Columns: 1 → 2 |
| 3 | (no heading) | 100 | — |
| 4 | LEARN MORE → | 84 | Heading: proxima-nova 16px → Sofia Sans 16px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 129px → 1139px |
| 5 | (no heading) | 100 | — |
| 6 | EXPLORE YOUR OPTIONS | 67 | Heading: adobe-garamond-pro 30px → Sofia Sans 16px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 219px → 1139px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPaddingMobile = 26
- Bring this section across (or check it was merged into another).
- Fewer columns: merge them into one stack column.

## /contact at 1440px — 64/100

Checks passed: 76% · screenshots 84% alike (two unrelated pages compare at about 55%).

Original: https://www.davidnicholmd.com/contact/  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Heading 2 size | 22px | 22px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 18px | same |
| Buttons letter spacing and case | 0.167em, uppercase | 0.167em, uppercase | same |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Section padding | 127px | 100px | same |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 40 | Background: #1f1f1f → #fafafa; Heading: proxima-nova 20px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 2 → 1; Image placement: center, 100% wide → none; Height: 2131px → 1432px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Give the section its own background color (style.background = { type: "color", color: "#1f1f1f" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).
- Adjust the stack column spans (image column) or the image's side.

## /contact at 390px — 38/100

Checks passed: 61% · screenshots 78% alike (two unrelated pages compare at about 65%) · 43% of its sections found.

Original: https://www.davidnicholmd.com/contact/  
Imported: /contact (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Heading 2 size | 22px | 22px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 16.9px | same |
| Buttons letter spacing and case | 0.167em, uppercase | 0.167em, uppercase | same |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 28.5px | 15.5px | **differs** |
| Button corners | 0px | 0px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | (no heading) | 100 | — |
| 3 | BEFORE YOUR VISIT: | 84 | Heading: proxima-nova 22px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 503px → 1303px |
| 4 | HOURS: | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 289px → 1303px |
| 5 | (no heading) | 0 | Present: Name First Name (required) Last Name (re → no matching section |
| 6 | (no heading) | 0 | Present: Email (required) Message (required) → no matching section |
| 7 | (no heading) | 0 | Present: SUBMIT → no matching section |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPaddingMobile = 29
- Bring this section across (or check it was merged into another).

## /david-nichol-md at 1440px — 0/100

Checks passed: 75% · screenshots 53% alike (two unrelated pages compare at about 55%) · 0% of its sections found.

Original: https://www.davidnicholmd.com/david-nichol-md/  
Imported: /david-nichol-md (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Buttons: present | proxima-nova 18px | not found | **differs** |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Content width | 1400px | 1344px | same |
| Section padding | 127px | 100px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 0 | Present: DAVID NICHOL MD → no matching section |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).

## /david-nichol-md at 390px — 38/100 (strict v3: 37/100)

Corrected scoring on this page:

- Section 2: columns counted on screen only (2 → 1 counted as 1 → 1; what's off screen or inside one slideshow or map isn't a column).

Checks passed: 71% · screenshots 76% alike (two unrelated pages compare at about 65%) · 60% of its sections found.

Original: https://www.davidnicholmd.com/david-nichol-md/  
Imported: /david-nichol-md (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 15px | 15.5px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | (no heading) | 75 | Italic lines: 1 → 0 |
| 3 | Dr. David Nichol | 84 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 203px → 1237px |
| 4 | (no heading) | 0 | Present:  → no matching section |
| 5 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 504px → 1237px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).
- Set the closing/pull line in italics (lead style).

## /health-information at 1440px — 51/100

Checks passed: 79% · screenshots 76% alike (two unrelated pages compare at about 55%).

Original: https://www.davidnicholmd.com/health-information/  
Imported: /health-information (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 2 size | 22px | 22px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 18px | same |
| Buttons letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Content width | 1400px | 1344px | same |
| Section padding | 127px | 200px | **differs** |
| Button corners | 300px | 0px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 58 | Background: #1f1f1f → #fafafa; Heading: proxima-nova 20px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 2 → 1 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 127
- choices.shape = "round"
- Give the section its own background color (style.background = { type: "color", color: "#1f1f1f" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /health-information at 390px — 45/100

Checks passed: 72% · screenshots 79% alike (two unrelated pages compare at about 65%) · 93% of its sections found.

Original: https://www.davidnicholmd.com/health-information/  
Imported: /health-information (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 2 size | 22px | 22px | same |
| Heading 3 size | 16px | 16px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 9px | 30.5px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | Health information | 81 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Height: 610px → 202px |
| 3 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 450px → 6905px |
| 4 | GENERAL DIET TIPS | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 321px → 6905px |
| 5 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 477px → 6905px |
| 6 | CARBOHYDRATES | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 858px → 6905px |
| 7 | FAT | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 1154px → 6905px |
| 8 | PROTEIN | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 401px → 6905px |
| 9 | FIBER | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 305px → 6905px |
| 10 | PHYTONUTRIENTS | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 791px → 6905px |
| 11 | VITAMINS AND MINERALS | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 181px → 6905px |
| 12 | (no heading) | 84 | Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 765px → 6905px |
| 13 | OTHER DIETARY SUPPLEMENTS | 67 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 620px → 6905px |
| 14 | WATER | 70 | Heading: proxima-nova 16px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 552px → 6905px |
| 15 | (no heading) | 80 | Height: 230px → 440px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPaddingMobile = 9
- Bring this section across (or check it was merged into another).

## /links at 1440px — 46/100

Checks passed: 71% · screenshots 74% alike (two unrelated pages compare at about 55%).

Original: https://www.davidnicholmd.com/links/  
Imported: /links (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 18px | same |
| Buttons letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Content width | 1400px | 1344px | same |
| Section padding | 127px | 276px | **differs** |
| Button corners | 300px | 0px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 37 | Background: #1f1f1f → #fafafa; Heading: proxima-nova 20px → EB Garamond 32px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 2 → 1 |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 127
- choices.shape = "round"
- Give the section its own background color (style.background = { type: "color", color: "#1f1f1f" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /links at 390px — 24/100

Checks passed: 80% · screenshots 68% alike (two unrelated pages compare at about 65%) · 50% of its sections found.

Original: https://www.davidnicholmd.com/links/  
Imported: /links (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 80px | 99px | same |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | Important websites | 94 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Text: adobe-garamond-pro 18px → EB Garamond 18px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Bring this section across (or check it was merged into another).

## /mental-health-information at 1440px — 41/100

Checks passed: 74% · screenshots 70% alike (two unrelated pages compare at about 55%).

Original: https://www.davidnicholmd.com/mental-health-information/  
Imported: /mental-health-information (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 32px | 32px | same |
| Heading 2 size | 22px | 22px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Buttons size | 18px | 18px | same |
| Buttons letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Navigation size | 18px | 18px | same |
| Navigation letter spacing and case | 0.111em, uppercase | 0.111em, uppercase | same |
| Site title size | 20px | 20px | same |
| Site title letter spacing and case | 0.1em, uppercase | 0.1em, uppercase | same |
| Content width | 1400px | 1344px | same |
| Section padding | 127px | 200px | **differs** |
| Button corners | 300px | 0px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | DAVID NICHOL MD | 44 | Background: #1f1f1f → #fafafa; Heading: proxima-nova 20px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Columns: 2 → 1; Height: 1848px → 916px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPadding = 127
- choices.shape = "round"
- Give the section its own background color (style.background = { type: "color", color: "#1f1f1f" }).
- Lay the text out in columns (a stack layout with more columns, or the text block's Columns style).

## /mental-health-information at 390px — 41/100

Checks passed: 77% · screenshots 76% alike (two unrelated pages compare at about 65%) · 75% of its sections found.

Original: https://www.davidnicholmd.com/mental-health-information/  
Imported: /mental-health-information (local preview)

| Check | Original | Imported | |
|---|---|---|---|
| Heading font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Heading 1 size | 30px | 30.1px | same |
| Heading 2 size | 22px | 22px | same |
| Body font | adobe-garamond-pro | EB Garamond (close stand-in) | close (85%) |
| Body text size | 18px | 18px | same |
| Label font | proxima-nova | Sofia Sans (close stand-in) | close (85%) |
| Site title size | 16px | 16.1px | same |
| Site title letter spacing and case | 0.125em, uppercase | 0.1em, uppercase | same |
| Section padding | 80px | 30.5px | **differs** |

| # | Section | Match | Differences |
|---|---|---|---|
| 1 | (no heading) | 0 | Present: I see patients at my home office in Boul → no matching section |
| 2 | Mental Health Information | 81 | Heading: adobe-garamond-pro 30px → EB Garamond 30.1px; Height: 725px → 202px |
| 3 | (no heading) | 80 | Height: 259px → 952px |
| 4 | COGNITIVE FUNCTION TEST | 84 | Heading: proxima-nova 22px → Sofia Sans 22px; Text: adobe-garamond-pro 18px → EB Garamond 18px; Height: 417px → 189px |

What would close the gap:

- Site Styles → choices.typography.heading = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.body = { family: "adobe-garamond-pro" } (Google Fonts), or upload it in Site Styles → Your fonts.
- Site Styles → choices.typography.label = { family: "proxima-nova" } (Google Fonts), or upload it in Site Styles → Your fonts.
- choices.layout.sectionPaddingMobile = 80
- Bring this section across (or check it was merged into another).

