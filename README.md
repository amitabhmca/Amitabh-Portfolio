# Amitabh Pandey — Portfolio

A one-page portfolio for **Amitabh Pandey**, a Singapore-based AI infrastructure and HPC professional (AI Factory · HPC · Platform architecture).

**Live site:** https://zhengyu89.github.io/Amitabh-Portfolio/ (available once GitHub Pages is enabled; the address changes if the repository moves to another account)

## What's on the page

| Section | Contents |
| --- | --- |
| Hero | Profile photo, introduction and his five active NVIDIA AI infrastructure certifications |
| 01 Certifications | Exam-based certifications in three tiers: AI factory / GPU cloud / HPC, cloud and cloud native, enterprise foundation |
| 02 Profile | About text and key facts |
| 03 Capabilities | A layer-by-layer skills stack, each layer linked to the certifications behind it |
| 04 Journey | Timeline from 2006 to today |
| 05 Selected work | Project case study and focus areas |
| 06 Recognition | Awards and LinkedIn recommendations |
| 07 Continuous learning | Course completions, kept separate from certifications |
| 08 Contact | Featured NVIDIA wallet, LinkedIn and Credly |

## Project layout

```
index.html      the whole site: HTML, inline CSS and inline JS
badges/         certification badge images (see badges/SOURCES.md for where each came from)
images/         profile photo shown in the hero
.nojekyll       tells GitHub Pages to serve the files as they are
```

There is no build step, no framework and no dependencies. The only external resource is Google Fonts (Bricolage Grotesque, Inter, DM Mono), and all asset paths are relative.

## Run it locally

Open `index.html` in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit http://localhost:8000.

## Deploy to GitHub Pages

1. In the repository, go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**, then `main` and `/ (root)`.
3. The site appears at `https://<owner>.github.io/<repo>/` after about a minute.

A repository named `<owner>.github.io` is served at the root, `https://<owner>.github.io/`. A custom domain keeps the address stable if the repository ever moves between accounts.

## Updating content

- **Certifications:** edit the cards in the `#credentials` section of `index.html`. Add the badge image to `badges/` and record its source in `badges/SOURCES.md`.
- **Dates and status:** the site shows only what is on his records. Expired certifications show the date they were earned, and only current ones are marked **Active**. Credentials with no known date show none.
- **Verification links:** NVIDIA certification badges link to their issuer verification pages on `credential.nvidia.com`. The NVIDIA wallet is featured in the top-right header and Contact, with stronger green styling than Credly. Other Credly-issued badges link to their public verification pages. Standard issuer artwork or product logos are not personal verification, so those cards are not labelled Verify.
- **Colours:** the blue theme is defined as variables at the top of the `<style>` block.

## Credentials data

NVIDIA certification images, issue and expiry dates, and verification links were checked against [his NVIDIA wallet](https://www.credential.net/profile/amitabhmca/wallet) on 6 November 2026. All five issuer badges are served locally, including NCP-ARI (issued 31 October 2026, expires 31 October 2028). The sixth wallet item is the 2020 Introduction to AI in the Data Center course, already listed under Continuous learning; it is not counted as an exam-based certification. Other badge images and verification links come from his public Credly wallet, https://www.credly.com/users/amitabh-pandey (downloaded October 2026). Certifications not issued through Credly (BeeGFS, WEKA, Bright Cluster Manager, RHCSA, VMware, Citrix, ITIL, EXIN) use official issuer artwork or logos. Jenkins credentials are intentionally left out.

## Before sharing widely

- The first-person text (hero, About, Contact) is draft wording and needs Amitabh's approval.
- Dates for RHCSA, VCP-Cloud, Citrix CCA, EXIN Cloud and WEKA are not available, so none are shown.
- Source and evidence notes are kept out of the repository on purpose (`doc/` is git-ignored).
