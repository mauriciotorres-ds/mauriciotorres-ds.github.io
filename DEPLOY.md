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

## Step 0: Your Headshot
Your headshot lives at **`assets/img/HeadShot02.JPG`** and is already wired into `index.html`.
- To swap it, replace that file (keep the same name) or add a new image and update the
  `<img src="assets/img/HeadShot02.JPG"` line in index.html to match.
- Any standard JPG/PNG works.

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
│       └── HeadShot02.JPG
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
