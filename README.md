# Your job board — how it works

Two files:
- `index.html` — the website itself. You never need to edit this.
- `jobs.json` — your local job listings. Edit this whenever you want to add, remove, or update a job.

International jobs load automatically from ReliefWeb's free public feed (engineering-related openings) — nothing to maintain there.

## To add a new local job

Open `jobs.json` and copy this block, then fill in your details:

```json
{
  "title": "Job title here",
  "company": "Company name",
  "location": "City, country",
  "posted": "2026-09-13",
  "last_date": "2026-09-30",
  "link": ""
}
```

Dates must be in `YYYY-MM-DD` format. Save the file — the website updates automatically.

## To put this online for free (GitHub Pages)

1. Go to github.com and create a free account if you don't have one.
2. Create a new repository (name it anything, e.g. `my-job-board`).
3. Upload `index.html` and `jobs.json` to it (there's an "Add file → Upload files" button).
4. Go to the repository's Settings → Pages.
5. Under "Source", choose the main branch and save.
6. GitHub gives you a link like `https://yourusername.github.io/my-job-board/` — that's your live website.

From then on, whenever you want to add a job: open `jobs.json` in GitHub (click the file, then the pencil/edit icon), add your entry, and commit the change. The live site updates within a minute or two.
