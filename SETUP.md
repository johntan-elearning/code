# Setup Guide

**For whoever is setting up this repository — follow these steps in order.**  
This guide assumes no prior GitHub experience. Every step is explained.

Estimated time: **30–45 minutes**

---

## What You Need

- A computer (any operating system)
- A web browser
- A free GitHub account (create one at https://github.com if you do not have one)
- The board files — all the HTML files from John Tan

---

## Step 1 — Create a GitHub Account (if you don't have one)

1. Go to https://github.com
2. Click **Sign up**
3. Choose a username. Suggested: `johntan-tvet`
4. Enter an email address and create a password
5. Complete the verification steps
6. You now have a GitHub account

---

## Step 2 — Create the Repository

1. Once logged in, click the **+** button in the top right corner
2. Select **New repository**
3. Fill in the details:
   - **Repository name:** `vocational-boards`
   - **Description:** `Vocational Snake and Ladders Board Game Suite — Open Educational Resource`
   - **Visibility:** Select **Public** ← this is essential for free GitHub Pages hosting
   - **Add a README file:** Leave **unchecked** — we will upload our own
4. Click **Create repository**

---

## Step 3 — Upload All Files

### Option A — Drag and Drop (Easiest, no technical knowledge needed)

1. On the repository page, you will see a message saying the repository is empty
2. Click **uploading an existing file** (blue link)
3. Drag ALL the files and folders from the package onto the upload area:
   - `README.md`
   - `LICENSE`
   - `ATTRIBUTION.md`
   - `SETUP.md` (this file)
   - `manifest.json`
   - `sw.js`
   - The entire `boards/` folder with all subfolders
4. Scroll down, add a commit message: `Initial upload — all 23 boards`
5. Click **Commit changes**

**Note:** GitHub's drag-and-drop upload handles folders. Drag the entire `boards/` folder.  
If it doesn't work with folders, use Option B below.

### Option B — GitHub Desktop (For folders, recommended)

1. Download GitHub Desktop from https://desktop.github.com
2. Install and sign in with your GitHub account
3. Click **Clone a repository** → find `vocational-boards` → choose a local folder
4. Copy all the files from the package into that local folder
5. In GitHub Desktop, you will see all the files listed as changes
6. Add a commit message: `Initial upload — all 23 boards`
7. Click **Commit to main**
8. Click **Push origin**

---

## Step 4 — Enable GitHub Pages

This is the step that makes the boards publicly accessible on the internet.

1. On the repository page, click **Settings** (top menu, far right)
2. In the left sidebar, click **Pages**
3. Under **Source**, click the dropdown and select **Deploy from a branch**
4. Under **Branch**, select **main** and keep `/ (root)` selected
5. Click **Save**
6. Wait 2–3 minutes
7. Refresh the page — you will see a green banner:  
   **"Your site is published at https://johntan-tvet.github.io/vocational-boards"**

**That URL is now permanent.** The boards are live.

---

## Step 5 — Test That It Works

Open this URL in your phone browser:  
`https://johntan-tvet.github.io/vocational-boards/boards/fnb/board1-orientation.html`

You should see the F&B Board 1 — Orientation board.

Test on a phone with mobile data (not WiFi) to verify it loads on 3G.

---

## Step 6 — Register a DOI via Zenodo (Optional but strongly recommended)

This gives the repository a permanent academic citation reference.

1. Go to https://zenodo.org
2. Log in with your GitHub account (click **Log in with GitHub**)
3. Go to your Zenodo profile → **GitHub** tab
4. Find `vocational-boards` in the list
5. Toggle it **ON**
6. Go back to GitHub and create a **Release**:
   - On the repository page, click **Releases** (right sidebar)
   - Click **Create a new release**
   - Tag: `v1.0`
   - Title: `Version 1.0 — Initial Release — 23 Boards`
   - Description: `First public release of the Vocational Snake and Ladders Board Game Suite. 23 boards across F&B Service, Kitchen, Technical and Vocational, Personal Care and Beauty, and Foundation pathways.`
   - Click **Publish release**
7. Zenodo automatically creates a DOI within minutes
8. That DOI goes into the APA citation and on John Tan's ORCID profile

---

## Step 7 — Update the README with the Real URLs

Once GitHub Pages is live and the DOI is registered:

1. Open `README.md` in the repository
2. Click the pencil (edit) icon
3. Replace all instances of `https://johntan-tvet.github.io/vocational-boards` with the actual URL shown in GitHub Pages Settings
4. Replace `[your-ORCID]` with John Tan's ORCID number
5. Replace `[your-profile]` with John Tan's ResearchGate profile name
6. Add the Zenodo DOI to the citation section
7. Click **Commit changes**

---

## Step 8 — Share the URL

The boards are now live. Share the main URL:

`https://johntan-tvet.github.io/vocational-boards`

Share individual board URLs via WhatsApp, QR code, or written on a whiteboard:

`https://johntan-tvet.github.io/vocational-boards/boards/fnb/board1-orientation.html`

---

## Moodle Embedding (For Trainers)

To embed a board inside a Moodle course:

1. In your Moodle course, click **Add an activity or resource**
2. Choose **Page**
3. Give it a name: e.g., `F&B Board 1 — Orientation`
4. In the **Page content** area, click the HTML source button (`<>`)
5. Paste this code (replace the URL for each board):

```html
<iframe 
  src="https://johntan-tvet.github.io/vocational-boards/boards/fnb/board1-orientation.html" 
  width="100%" 
  height="700px" 
  frameborder="0"
  allowfullscreen>
</iframe>
```

6. Click **Save and display**

The board now appears inside Moodle. Students play it without leaving the course.

---

## If You Get Stuck

Common issues:

**The site is not showing after enabling GitHub Pages:**  
Wait 5 minutes and refresh. GitHub Pages takes a few minutes the first time.

**The boards folder did not upload correctly:**  
Use GitHub Desktop (Option B above) — it handles folders more reliably than drag-and-drop.

**The URL shows a 404 error:**  
Check that the file is in the correct folder path. The URL must match the exact folder and file name.

**Zenodo is not finding the repository:**  
Make sure the repository is Public (not Private). Zenodo cannot access private repositories.

---

*This setup guide was prepared as part of the Friends International / Mith Samlanh eLearning Architecture Project, May 2026.*  
*John Tan · Technical Practitioner and Mentor · TVET and Tourism Education*
