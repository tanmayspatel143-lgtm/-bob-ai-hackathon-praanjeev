# How to Submit Your Hackathon Entry

Follow these steps to set up your submission repository correctly.
The judges depend on this structure to review your entry — deviations may affect your score.

---

## Step 1 — Fork This Template

1. Click the **"Use this template"** button at the top of this repository
   (or **Fork** if you prefer)
2. Name your repository: `bob-ai-hackathon-[your-team-name]`
3. Set visibility to **Public** so judges can access it
4. Click **Create repository**

---

## Step 2 — Clone Your Fork Locally

```bash
git clone https://github.com/[your-org]/bob-ai-hackathon-[your-team-name].git
cd bob-ai-hackathon-[your-team-name]
```

---

## Step 3 — Fill in the Required Files

Work through these files in order:

### 3a. `submission.yaml` ← **Start here**

This is the most important file. Fill in **every field marked `# REQUIRED`** and read the inline comments.

### 3b. `README.md`

Replace every `[placeholder in brackets]` with your actual content.

### 3c. `docs/`

Fill in all four documentation files: problem statement, solution overview, architecture, and setup guide.

### 3d. `src/`

Put all source code inside `src/`. Copy `src/.env.example` to `.env` and add environment variables. **Never commit a real `.env` file.**

### 3e. `demo/`

Replace the demo video placeholder, add the live demo URL (or `NOT DEPLOYED`), and add 3+ screenshots.

### 3f. `presentation/`

Add your slide deck as `presentation/slides.pdf` (preferred) or `.pptx`.

---

## Step 4 — Verify Your Submission Passes Validation

Every push triggers the **Validate Submission** GitHub Action automatically.

To check manually, open the repo's **Actions** tab and inspect the latest **Validate Submission** run.

You can also run validation locally with `yq '.' submission.yaml`.

---

## Step 5 — Submit Your Repository URL

Once validation passes, copy your repository URL and submit it via the official entry form.

> ⚠️ Submissions after the deadline will not be reviewed.

---

## Checklist Before You Submit

- [ ] `submission.yaml` — all required fields filled
- [ ] `README.md` — no `[placeholder]` text remaining
- [ ] `docs/setup-guide.md` — someone else can run your project
- [ ] `src/` — all source code committed; no `node_modules` or `.env`
- [ ] `demo/demo-video-link.txt` — real video URL
- [ ] `demo/screenshots/` — at least 3 screenshots
- [ ] `presentation/slides.pdf` — slide deck present
- [ ] GitHub Actions validation is green
- [ ] Repository is **Public**
- [ ] Entry form submitted before the deadline
