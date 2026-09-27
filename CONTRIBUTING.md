# Contributing

Thanks for helping improve the guide. A few ground rules:

- **Scope**: one topic per file under `topics/`. Keep each topic readable in ~10 minutes.
- **Template**: follow the structure already used in existing topic files (Why it matters, Core concepts, Mental model, Interview questions, Watch, Further reading).
- **Links must be real**: only link to YouTube videos and articles you have personally verified exist (open the URL, confirm the title/content). Never guess a video ID or URL. Prefer Khan Academy, MIT OpenCourseWare, Wharton/Cornell course material, and other reputable educational sources — but any verified source is fine. If you are unsure of an exact URL, omit the video rather than invent one.
- **No invented product direction**: this guide covers accounting and financial-statement fundamentals for investment-banking and markets interview prep, plus self-study. It is not a CPA exam review, not a tax reference, not a consolidation/merger-acquisition guide, and not a quiz or auth site. If you want to propose a new topic or reorganize the curriculum, open an issue first.
- **Accounting rigor, not bookkeeping drills**: the bar is that a CS/stats/econ or Wharton QF student can read a 10-K, reason about *why* a number moved, and hold a conversation with an analyst. Debits/credits appear as conceptual bookkeeping only. Don't add journal-entry exercises, T-account drills, or US GAAP codification detail.
- **Keep topics tight**: prefer accurate intuition and interview-ready answer keys over encyclopedic coverage. Don't invent extra scope (no data feeds, no interactive ratio calculators, no login).
- **Local preview**:
  ```bash
  bundle install
  bundle exec jekyll serve
  ```
  Then open `http://localhost:4000`.
- **Pull requests**: keep them focused (one topic or fix per PR) and describe what changed and why.
