# HW5 Setup Instructions

Follow these steps in order. Each step takes only a minute or two.

---

## Step 1 – Download all these files

Download / clone this folder. You will see this structure:

```
hw5/
├── _config.yml
├── Gemfile
├── index.html
├── _layouts/
│   ├── home.html
│   └── post.html
├── _posts/
│   └── 2026-04-16-hw5.md
├── assets/
│   └── json/
│       ├── chart1.json   ← placeholder, replaced in Step 2
│       └── chart2.json   ← placeholder, replaced in Step 2
└── python_notebooks/
    └── hw5_licenses.ipynb
```

---

## Step 2 – Run the Python notebook to generate the charts

1. Open `python_notebooks/hw5_licenses.ipynb` in Jupyter or VS Code.
2. Run all cells top to bottom.
3. The last two cells save `chart1.json` and `chart2.json` into `assets/json/`.  
   *(The save path is `'../assets/json/chart1.json'` — this works if you open the notebook from inside `python_notebooks/`.)*
4. Confirm `assets/json/chart1.json` and `chart2.json` have been updated (they should now be large JSON files, not tiny placeholders).

> **Tip:** If you get a "rows larger than maximum" error, make sure `alt.data_transformers.disable_max_rows()` ran (it's in the first code cell).

---

## Step 3 – Upload everything to your GitHub Pages repo

Your GitHub Pages repo is **SamuelSokolovsky/SamuelSokolovsky.github.io**.

1. Go to https://github.com/SamuelSokolovsky/SamuelSokolovsky.github.io
2. Upload **all** the files/folders from `hw5/` into the **root** of your repo.  
   The easiest way: use "Add file → Upload files" in GitHub's web UI, or drag-and-drop.  
   You can also use git:
   ```bash
   git clone https://github.com/SamuelSokolovsky/SamuelSokolovsky.github.io
   # copy all hw5/ contents into the cloned folder
   git add .
   git commit -m "Add HW5 Jekyll site with licenses visualizations"
   git push
   ```
3. **Important:** Make sure `_config.yml` ends up in the repo **root** (not inside a subfolder), otherwise Jekyll won't build.

---

## Step 4 – Enable Jekyll on GitHub Pages (if not already)

1. Go to your repo on GitHub → **Settings** → **Pages**.
2. Under "Build and deployment", set Source to **Deploy from a branch**.
3. Set Branch to **main** (or master) and folder to **/ (root)**.
4. Click **Save**.
5. Wait ~60 seconds, then visit **https://SamuelSokolovsky.github.io** — you should see the home page listing your HW5 post.

---

## Step 5 – Verify the post renders correctly

Click the HW5 post link on the home page. You should see:
- Chart 1 (interactive line chart) rendered above the first paragraph
- Chart 2 (bar chart) rendered above the second paragraph
- Two buttons: "The Data" and "The Analysis"

If the charts show a blank box, wait another minute and hard-refresh (Ctrl+Shift+R).

---

## Step 6 – Submit

Paste **https://SamuelSokolovsky.github.io** into the PrairieLearn submission box.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| Charts don't appear | Check that `assets/json/chart1.json` and `chart2.json` are committed and not the placeholder versions |
| 404 on the post | Make sure the `_posts/` folder was uploaded and the filename starts with a date like `2026-04-16-hw5.md` |
| Jekyll not building | Make sure `_config.yml` is in the repo root; check the Actions tab for build errors |
| "The Analysis" button 404 | After uploading, the notebook URL should be `https://github.com/SamuelSokolovsky/SamuelSokolovsky.github.io/blob/main/python_notebooks/hw5_licenses.ipynb` — GitHub renders notebooks automatically |
