# ⛳ GHIN Dashboard

A clean, private web dashboard for viewing your GHIN scores, handicap trend, and club members' handicaps — hosted for free on GitHub Pages.

---

## Features

- **My Scores** — full score history with course name, tees, rating/slope, and differentials
- **Handicap Trend** — rolling handicap index chart + score differential bar chart
- **Club Members** — view all club members' handicap indexes with search/filter

---

## Setup (GitHub Pages)

### Step 1 — Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in
2. Click **New repository** (green button, top right)
3. Name it something like `ghin-dashboard`
4. Set it to **Public** (required for free GitHub Pages)
5. Click **Create repository**

### Step 2 — Upload the file

1. On your new repo page, click **Add file → Upload files**
2. Drag and drop `index.html` into the upload area
3. Scroll down and click **Commit changes**

### Step 3 — Enable GitHub Pages

1. Go to your repo **Settings** (top menu)
2. Click **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Set Branch to **main** and folder to **/ (root)**
5. Click **Save**

After ~1 minute, your site will be live at:
```
https://YOUR-USERNAME.github.io/ghin-dashboard/
```

---

## How to Use

1. Open your GitHub Pages URL
2. Enter your **GHIN username and password** (same as ghin.com or the GHIN app)
3. Your scores and club members load automatically

**Your credentials are never stored** — they're used only for the GHIN API call in your browser session. When you close the tab, they're gone.

---

## Notes & Limitations

- The GHIN API endpoints used here are the same ones the official GHIN app uses. They are not officially documented for third-party use, so behavior may change if GHIN updates their API.
- Club members shown are those accessible via your GHIN account (typically your home club's roster).
- Handicap trend is calculated from your score differentials using the WHS formula (best 8 of last 20 × 0.96).

---

## Privacy

- This is a **static HTML file** — there is no server, no database, no tracking.
- Your GHIN credentials are sent directly from your browser to `api.ghin.com` and nowhere else.
- If you want extra privacy, you can make the GitHub repo **Private** and use GitHub Pages with a paid plan, or just open the `index.html` file locally in your browser without hosting it at all.

---

## Updating

To update the dashboard in the future, just upload a new `index.html` to your GitHub repo the same way — it will replace the old one automatically.
