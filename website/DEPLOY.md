# Deploying Your Site to GitHub Pages

## Folder Structure
```
website/
├── index.html          ← Your entire site (one file)
├── assets/
│   ├── resume.pdf      ← Your resume (swap with latest version anytime)
│   └── img/
│       └── headshot.jpg  ← ⚠️ YOU NEED TO ADD THIS (see Step 0 below)
```

---

## Step 0: Add Your Headshot
Save your headshot photo as **`headshot.jpg`** inside the `assets/img/` folder.
- Any standard JPG/PNG works. Name it exactly `headshot.jpg`.
- If you use a PNG, change line ~247 in index.html:
  `<img src="assets/img/headshot.jpg"` → `<img src="assets/img/headshot.png"`

---

## Step 1: Copy Files to Your GitHub Pages Repo

Your site lives at: **https://mauriciotorres-ds.github.io**
That means your GitHub repo name is: **`mauriciotorres-ds.github.io`**

Copy EVERYTHING in this `website/` folder into the ROOT of that repo.
The repo should look like:
```
mauriciotorres-ds.github.io/
├── index.html
├── assets/
│   ├── resume.pdf
│   └── img/
│       └── headshot.jpg
```

---

## Step 2: Push to GitHub

In terminal (from inside the repo folder):
```bash
git add .
git commit -m "New personal site"
git push
```

GitHub Pages will automatically rebuild. Your site will be live at:
**https://mauriciotorres-ds.github.io** within ~60 seconds.

---

## Updating Your Resume
Just replace `assets/resume.pdf` with your new resume, keep the same filename, and push again.

## Updating Any Content
All content is in `index.html`. Search for the text you want to change and edit it directly.
