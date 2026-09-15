# Genesis — built in ChatGPT, zero Codex

A live visualization of this repository's own commit history, rendered as a two-arm spiral galaxy inspired by the GPT Astra key visual.

- Built directly in ChatGPT with the GitHub connector
- Codex usage: 0 tokens
- Raw WebGL2 only; Canvas 2D fallback
- No external libraries, frameworks, CDNs, or build step
- Each repository commit becomes a bright “main star” on one of the spiral arms
- New commits ignite when detected
- Commit history is refreshed every 75 seconds with `ETag` / `If-None-Match`

The page reads public commit data from:

`https://api.github.com/repos/blessing1031r-dotcom/astra-no-codex/commits?per_page=100`

Open `index.html` directly or publish the repository with GitHub Pages.
