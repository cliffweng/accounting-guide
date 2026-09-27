# STATUS

## Pull request

**https://github.com/cliffweng/accounting-guide/pull/1**

- Draft, open, **not merged**
- `main` ← `owen/init-accounting-guide`
- 21 files, +1428 / −0

## Branch state

| | |
|---|---|
| Branch | `owen/init-accounting-guide` |
| Commit | `ce809d3` — *Add accounting & financial statements study guide* |
| Base | `main` @ `61f8519` — *Initialize repository* (empty root commit) |
| Deployed to | not yet — Pages builds after merge to `main` |

## Delivered

- 14 topics in `topics/`, `nav_order` 2–15, each with why it matters → core
  concepts → mental model → interview Q&A with answer keys → verified YouTube
  watch list → further reading. Topic 14 carries the 🎯 Frequent badge.
- Site files: `_config.yml`, `Gemfile`, `LICENSE`, `CONTRIBUTING.md`,
  `README.md`, `index.md`, `.gitignore`.
- Every page scoped to ≤10 min (badges run 6–10 min).

## Verification

- **Build:** clean `JEKYLL_ENV=production bundle exec jekyll build`
  (Jekyll 4.4.1, just-the-docs 0.12.0). 15 HTML pages generated. Remaining
  output is Sass deprecation warnings from the upstream theme, not site content.
- **Internal links:** 342/342 resolve in built HTML, validated after `baseurl`
  resolution. This surfaced a real defect — 7 `../topics/...` links on the home
  page resolved outside `/accounting-guide` and would have 404'd in production.
  Fixed to `topics/...`.
- **External links:** 49/49 return HTTP 200 (Khan Academy, Wall Street Prep,
  Investopedia, YouTube). Two repaired during review: a malformed video ID in
  topic 03, and a dead Investopedia slug in topic 08.
- **Structure:** 14 permalinks, `nav_order` sequence, required sections, badge
  vs. home-page table consistency, and front matter all verified programmatically.

## Notes / caveats

- `main` did not exist on the remote (the repo had no commits at all), so it was
  initialized with an **empty root commit** to give the PR a base. No site content
  is on `main`. `main` was never force-pushed.
- The feature branch was rebased onto `main` and force-pushed once with
  `--force-with-lease` to establish shared history. `main` is untouched.
- `Gemfile.lock` is gitignored, matching the sibling guides, so Pages resolves
  gems from `Gemfile` at build time.
- Intentionally uncommitted: `OPENCODE_TASK.md`, `REFERENCE_*.txt`, `_ref/`.
- `https://cliffweng.github.io/accounting-guide/` currently 404s — expected, as
  the site is not deployed until this PR merges.
- Git identity was unset, so a repo-local identity (`Cliff Weng`,
  `7596956+cliffweng@users.noreply.github.com`) was configured for this
  repository only. Global config untouched.
- Ruby 3.3.8 was installed system-wide via apt in the dev sandbox to run the
  build; gems are vendored into the gitignored `vendor/`.
