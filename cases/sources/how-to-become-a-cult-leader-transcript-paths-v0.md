# How to Become a Cult Leader — Transcript Paths (v0)

Purpose: identify practical ways to obtain transcript-equivalent text for the Netflix docuseries **How to Become a Cult Leader**.

Status: partially solved.

---

## What I confirmed

### Netflix title page is reachable
Title:
- `How to Become a Cult Leader`
- Netflix title id: `81596972`

Visible from the public title page:
- 6 episodes
- episode titles + descriptions
- subtitles available on Netflix in:
  - English
  - Spanish (Latin America)
  - French
  - Chinese (Simplified)
  - Chinese (Traditional)

Episode list confirmed:
1. `Build Your Foundation`
2. `Grow Your Flock`
3. `Reform Their Minds`
4. `Promise Eternity`
5. `Control Your Image`
6. `Become Immortal`

---

## Best transcript paths found

### Path A — Full episode transcript mirrors (best if accessible)
Search surfaced a transcript mirror:
- `https://tvshowtranscripts.ourboard.org/viewforum.php?f=1940`
- example result: episode transcript page for `s01e01 - Build Your Foundation`

Current blocker:
- automated access hits Cloudflare bot verification (`Performing security verification` / `Just a moment...`)

What this means:
- the transcripts probably exist there
- but I could not programmatically fetch them from the current lane

---

### Path B — Subtitle sites (strong fallback)
Search surfaced subtitle sources:
- Addic7ed show page: `https://www.addic7ed.com/show/9501`
- Addic7ed episode result pages for specific episodes
- OpenSubtitles search page for the series

Current state:
- Addic7ed show page is reachable enough to confirm the show exists there
- but episode content / subtitle loads were unstable (`Server too busy` / odd 304 behavior on direct episode fetches)
- OpenSubtitles result exists in search, but was not fetched in this pass

What this means:
- subtitle files likely exist and are probably the easiest transcript-equivalent source
- but the current automation path did not fully pull them down yet

---

### Path C — Netflix captions via authenticated browser session (most direct)
Because the Netflix public page clearly exposes subtitle availability, the most direct extraction path is:
1. access the show in an authenticated browser session
2. play each episode with English subtitles / CC enabled
3. capture subtitle text live or from network / DOM
4. stitch into transcript files per episode

Current blocker:
- current managed browser is not signed into Netflix
- no attached user browser session was available in this pass

What this means:
- this path is very likely workable
- but it needs either Netflix login in the automation lane or a user-attached browser tab

---

## Recommended next move

### Fastest likely success path
Use an authenticated user browser session on Netflix and scrape captions live while the episode plays.

Minimal human step if needed:
- open the Netflix episode in your browser
- make sure subtitles are enabled in English
- attach the browser tab if using the OpenClaw Browser Relay / Chrome extension lane

Why this is the best lane:
- it bypasses transcript-mirror Cloudflare problems
- it uses Netflix’s own caption track
- it should produce transcript-equivalent text even if subtitle sites are flaky

---

## Backup path
If live Netflix extraction is inconvenient, keep pushing on subtitle mirrors:
1. Addic7ed
2. OpenSubtitles
3. transcript mirror forum pages

---

## Bottom line

A transcript path **does exist**.

Most promising options, in order:
1. **scrape live Netflix captions in an authenticated browser session**
2. **pull subtitle files from Addic7ed / OpenSubtitles**
3. **use the tvshowtranscripts mirror if Cloudflare can be cleared**
