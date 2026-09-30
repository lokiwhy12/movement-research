# Synanon draft sources

Lives at: `cases/synanon.SOURCES.md`.
What this is for: URLs actually opened or used in the 2026-09-30 draft-and-hold pass. If a number or policy is not on a page listed here, the packet marks it “not found in this pass.” Search snippets are not full opens. Archive path claimed for the packet: `cases/synanon.target-packet.md`.

Created: 2026-09-30 (CT)
Status: finish-gated SIGN as written 2026-09-30 CT; filing. Needs counsel review.

---

## Primary / encyclopedia pages opened (full)

- https://en.wikipedia.org/wiki/Synanon — full HTML via WebFetch (founding, Game, stages, church, Marines, Morantz, pleas, IRS, dissolution, lineage)

## Journalism / critique pages opened (full)

- https://www.lamag.com/citythinkblog/synanon-cult/ — Hillel Aron, Apr 23, 2018 (WebFetch); richest single narrative + asset/price figures
- https://www.motherjones.com/politics/2007/08/cult-spawned-tough-love-teen-industry/ — Maia Szalavitz, 2007 (WebFetch)
- https://www.latimes.com/archives/la-xpm-2001-oct-17-cl-58045-story.html — Jonathan Kirsch on Janzen book, Oct 17, 2001 (WebFetch)
- https://www.latimes.com/california/story/2022-10-28/paul-morantz-dies-l-a-attorney-nearly-killed-when-cult-planted-rattlesnake-in-mailbox — Steve Marble, Oct 28, 2022 (curl full HTML)
- https://www.latimes.com/california/story/2024-05-29/synanon-rattlesnake-mailbox — Christopher Goffard, May 29, 2024 (curl full HTML)
- https://www.sfgate.com/sf-culture/article/bay-area-family-rescued-children-synanon-19402428.php — Katie Dowd, Apr 21, 2024 (curl full HTML; WebFetch JS-walled — count curl open)
- https://www.thedailybeast.com/a-violent-deadly-cult-with-forced-abortions-and-shades-of-scientology — Nick Schager, Apr 24, 2020 (curl; pop-culture / Oxygen gloss — secondary)

## Government / legal primary opened (full)

- https://www.irs.gov/pub/irs-tege/eotopicb90.pdf — 1990 EO CPE Text, “Taxation of Revoked Tax-Exempt Organizations: The Synanon Case” (curl + pdftotext)

## Academic / memoir PDFs opened (full)

- https://deriu82xba14l.cloudfront.net/file/595/2002-Yablonsky-What-Ever-Happened-to-Synanon.pdf — Lewis Yablonsky, *Criminal Justice Policy Review* 2002 reprint PDF
- https://scholarworks.gvsu.edu/cgi/viewcontent.cgi?article=1620&context=communalsocieties — Ellen Broslovsky memoir in *Communal Societies* + Janzen editor intro PDF

## Nostalgia / secondary voice opened (partial; labeled)

- https://synanon.com/the-game/ — memorial site with attributed Dederich quotes on Game origin / father principle (WebFetch + curl; **not** contemporaneous official org docs)

## In-repo method shape referenced (not cloned as Synanon content)

- Osho / OneTaste filled-draft packet structure under `/workspace/movement-research-drafts/` as quality bar
- `movement-research-method` checklist shape for section order

## Attempted; blocked or not fully retrieved this pass

- https://www.paulmorantz.com/cult/the-history-of-synanon-and-charles-dederich/ — **403 Forbidden** (curl and WebFetch)
- https://law.justia.com/cases/federal/appellate-courts/F2/820/421/115606/ — **403** on curl; WebFetch timeout
- https://www.nytimes.com/1997/03/04/us/charles-dederich-83-synanon-founder-dies.html — timeout / thin stub
- https://press.jhu.edu/books/title/2826/rise-and-fall-synanon — **Cloudflare block** on WebFetch
- https://www.salon.com/1999/03/30/synanon/ and nearby Salon URLs — **404**
- https://breakingcodesilence.org/playing-the-game-the-origins-and-impact-of-synanon/ — **404**
- https://gizmodo.com/the-man-who-fought-the-synanon-cult-and-won-1632925562 / paleofuture mirror — **404** / homepage redirect
- Time.com “Synanon Sequel” (1980) — wrong article body retrieved on tried URL; **not counted**
- Full Janzen *Rise and Fall of Synanon* monograph — not opened as book PDF
- Marin County 1978 grand jury report primary — not retrieved
- web.archive.org Morantz history capture — empty response this pass

## Access notes

- Keep **insider/nostalgia voice** (synanon.com; Broslovsky memoir affection) separate from **external reporting** (LAT, LA Mag, Mother Jones, SFGate) and from **government/court paraphrase** (IRS CPE, Wikipedia plea/tax summary).
- Wikipedia Charles Dederich standalone fetch resolved to the Synanon article in this environment; biography facts taken from Synanon page + LA Mag oral-history paraphrase.
- Square Game cash fees and early residential tuition schedules: **not found as sticker tables** on pages opened — marked unpublished/historical-unknown in packet §8.
- Asset figures ($22M / $8M / $30M+ / $17M back taxes / $500k bonus) are attributed to the specific opened pages above; do not invent inflation conversions as facts unless the source states them (LA Mag states ~$400k modern equivalent for $100k salary — optional color only).
- Daily Beast contains dramatized errors risk (e.g. role of Morantz); packet prefers LAT / LA Mag / Wikipedia / IRS for contested legal facts.
- SFGate WebFetch returned JS interstitial; curl retrieved usable article body — counted as full open via curl.
- No git commit, PR, or outbound message performed for this draft.
