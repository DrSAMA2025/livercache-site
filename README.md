# LiverCache 🧊
### *Where shelved liver science gets cached.*

> An open, community-driven archive for unpublished, negative, and shelved hepatology research — making dark data visible, citable, and reusable.

---

## What Is This Repo?

This repository currently hosts the **design specification and visual brief** for the LiverCache website. It is the working document Somaya and Scottie are using to align on the site's layout, content, and technical architecture before development begins.

The live spec is viewable at: **`https://[your-username].github.io/livercache-site`**
*(Update this URL once GitHub Pages is enabled — see setup instructions below.)*

---

## For Scottie — How to Edit the Spec

The entire design spec lives in one file: **`index.html`**

### Option A: Edit directly on GitHub (no setup needed)
1. Open `index.html` in this repo
2. Click the **pencil icon** (top right of the file view) to edit
3. Make your changes
4. Click **"Commit changes"** at the bottom
5. The live site updates automatically within ~30 seconds

### Option B: Edit locally (recommended for bigger changes)
```bash
# Clone the repo
git clone https://github.com/[your-username]/livercache-site.git
cd livercache-site

# Open in VS Code
code .

# Install the "Live Server" extension in VS Code
# Right-click index.html → "Open with Live Server"
# You'll see live changes in your browser as you edit

# When done
git add .
git commit -m "design: [describe your change]"
git push
```

### What's Easy to Change

All visual styles are controlled by **CSS variables** at the top of `index.html` (around line 10). You can retheme the entire site by changing just these values:

```css
:root {
  --bg: #f5f0e8;        /* Page background */
  --ink: #1a1208;       /* Primary text / dark elements */
  --rust: #c4401a;      /* Primary accent color */
  --amber: #e8883a;     /* Secondary accent */
  --sage: #4a6741;      /* Tertiary accent */
  --cream: #faf7f0;     /* Section backgrounds */
  --muted: #8a7d6b;     /* Secondary text */
  --border: #d8cfc0;    /* Borders and dividers */
}
```

**Other easy edits:**
- All body copy and headings are plain HTML — just find and replace text
- The 3 page wireframes are in tabs — each is a `<div id="spec-home/browse/submit">`
- The roadmap items are `<div class="roadmap-item">` blocks — add/remove freely
- Fonts are loaded from Google Fonts — swap the import URL to change typography

---

## Enabling GitHub Pages (Somaya — do this once)

1. Go to this repo on GitHub
2. Click **Settings** (top menu)
3. In the left sidebar, click **Pages**
4. Under "Source", select **Deploy from a branch**
5. Choose **main** branch, **/ (root)** folder
6. Click **Save**
7. After ~1 minute, your site will be live at `https://[your-username].github.io/livercache-site`

---

## Project Overview

| | |
|---|---|
| **Project Name** | LiverCache |
| **Tagline** | Where shelved liver science gets cached |
| **Domain** | Hepatology / Open Science |
| **Access Model** | Open · CC BY 4.0 |
| **Status** | Pre-launch · Design Phase |

### The Problem
Publication bias leaves a graveyard of valuable hepatology findings invisible to the scientific community. Null results, abandoned trials, negative findings, and shelved datasets are never published — yet they contain critical information that could prevent duplicated effort and wasted funding.

### The Solution
LiverCache is a free, open-access archive where hepatology researchers can submit and discover unpublished work. Every entry is citable (DOI via Zenodo), versioned (GitHub), and licensed for reuse (CC BY 4.0).

### Planned Website Structure
| Page | Purpose |
|---|---|
| **Homepage** | Mission, recent submissions, how to contribute |
| **Browse** | Search and filter all cached entries |
| **Submit** | Submission form for new entries |

### Proposed Tech Stack
| Tool | Role |
|---|---|
| GitHub Pages | Static site hosting (free) |
| Google Forms | Submission intake |
| Zenodo / OSF | File hosting + DOI issuance |
| Markdown + frontmatter | Entry structure per submission |
| CC BY 4.0 | Content license |
| MIT | Code license |

---

## Team

| Name | Role |
|---|---|
| **Somaya Albhaisi** | GI/Liver Fellow · Project Lead & Founder |
| **Scottie Enriquez** | Computer Science Lead · Co-Founder |

---

## Roadmap

- **Week 1:** GitHub org, repo, governance docs, basic site live
- **Month 1:** Full 3-page site, Google Form live, soft launch via listservs + social
- **Month 3–6:** First curated entries, first DOIs via Zenodo, volunteer curators recruited
- **Year 1:** Impact evaluation, grant applications, society partnerships (AASLD/EASL)

---

## License

- **Content:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Code:** [MIT](https://opensource.org/licenses/MIT)

---

*LiverCache is independent and not affiliated with Arcadia Science or any existing initiative.*
