# Bob AI Innovation Hackathon Submission Template — Complete Guide

This guide explains how to structure and submit a hackathon entry using this repository template.

## Table of Contents

1. Overview
2. Getting Started
3. Repository Structure
4. File-by-File Walkthrough
5. Automated Validation
6. Submission Checklist
7. Evaluation
8. Common Mistakes
9. FAQ

## 1. Overview

The template gives every team a consistent repository so judges can find the required material and automated validation can check structural completeness.

**One template → one repo per team. Do not share repos across teams.**

## 2. Getting Started

Create or use the repository, fill in the required fields in `submission.yaml`, replace README placeholders, add your source code under `src/`, complete the documentation, add demo evidence, and push the finished submission.

## 3. Repository Structure

```text
├── submission.yaml
├── README.md
├── src/
│   ├── .env.example
│   └── README.md
├── docs/
│   ├── problem-statement.md
│   ├── solution-overview.md
│   ├── architecture.md
│   └── setup-guide.md
├── demo/
│   ├── demo-video-link.txt
│   ├── live-demo-url.txt
│   └── screenshots/
├── presentation/
├── CONTRIBUTING.md
├── .gitignore
└── .github/workflows/validate.yml
```

## 4. File-by-File Walkthrough

### `submission.yaml`

This is the structured metadata used by evaluators. Fill every field marked `# REQUIRED`. The track must be one of `AI`, `DevOps`, `Sustainability`, or `Open`.

### `README.md`

Use this as the human-readable front page. Replace all placeholders with your actual project information, setup steps, demo links, limitations, and strongest achievement.

### `docs/`

- `problem-statement.md`: explain the audience, pain point, impact, and shortcomings of existing solutions.
- `solution-overview.md`: explain what you built, how it works, key decisions, and IBM technology usage.
- `architecture.md`: include a technical diagram, components, data flow, security, and scalability notes.
- `setup-guide.md`: provide exact prerequisites, environment variables, installation, run, test, and troubleshooting steps.

### `src/`

Place all project source code here. Never commit real `.env` credentials, `node_modules`, virtual environments, or build artifacts.

### `demo/`

Provide a real 3–5 minute demo video link, an optional live deployment URL, and at least three screenshots of the running application.

### `presentation/`

Add the final slide deck as `slides.pdf` or `slides.pptx`.

## 5. Automated Validation

Every push triggers `.github/workflows/validate.yml`. It checks that required files exist, YAML is parseable, required submission fields are populated, source code exists, the demo video link is updated, and README placeholders are replaced.

Open the repository's **Actions** tab to inspect the latest validation run.

## 6. Submission Checklist

- [ ] Required `submission.yaml` fields filled
- [ ] README placeholders replaced
- [ ] Four documentation files completed
- [ ] Source code committed under `src/`
- [ ] Real demo video link provided
- [ ] At least three screenshots added
- [ ] Presentation added
- [ ] No secrets or build artifacts committed
- [ ] Validation workflow passes
- [ ] Repository is public

## 7. Evaluation

Entries may be evaluated on technical implementation quality, innovation and differentiation, understanding of the problem, working functionality, IBM Bob integration, and documentation/reproducibility.

## 8. Common Mistakes

Avoid leaving `[placeholder]` text, committing `.env` secrets, submitting an empty `src/`, using a placeholder demo URL, omitting screenshots, or changing the expected filenames.

## 9. FAQ

**Can we use our own `src/` structure?** Yes. The structure inside `src/` is up to the team.

**Can we add extra files?** Yes, provided required files remain in their expected locations.

**What if the demo is not deployed?** Write `NOT DEPLOYED` in `demo/live-demo-url.txt` and ensure the setup guide lets judges run it locally.

**Can we update the repository after the first push?** Yes, continue pushing changes until the submission deadline.
