# Genesis — built in ChatGPT, zero Codex

A live visualization of Roku's public GitHub commit history, rendered as a two-arm spiral galaxy inspired by the GPT Astra key visual.

- Built directly in ChatGPT with the GitHub connector
- Codex usage: 0 tokens
- Raw WebGL2 only; Canvas 2D fallback
- No external libraries, frameworks, CDNs, or build step
- Every public commit attributed to `blessing1031r-dotcom` becomes a bright clickable “main star”
- Commits are collected across the account's public repositories and merged chronologically
- Newer commits sit closer to the core; older commits move toward the outer arms
- Private repositories are intentionally excluded from the public visualization
- New commits in this Genesis repository ignite when detected
- The live repository is checked every 75 seconds with `ETag` / `If-None-Match`
- Full public history is cached locally for 10 minutes to avoid wasting GitHub API rate limit

The page reads public data from GitHub's REST API, beginning with:

`https://api.github.com/users/blessing1031r-dotcom/repos?per_page=100&type=owner`

Open `index.html` directly or publish the repository with GitHub Pages.
