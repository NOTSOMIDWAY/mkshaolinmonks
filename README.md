# MK Shaolin Monks Research Archive

**Created by OGmidway** | [Live Site](https://ogmidway.github.io/mkshaolinmonks)

The first publicly documented reverse-engineering archive for **Mortal Kombat: Shaolin Monks (2005)**, built on the **Paradox Engine** by Midway Studios LA.

## What's Here

- 🔊 **Audio Player** — 103 decoded ADX audio files from GAMEDATA.WAI
- 📂 **File Formats** — PWF, EWDF, CRI AFS, CRI ADX, ps2_DTPK documented
- 🖼 **Assets Gallery** — All extracted game assets
- 📜 **Research Log** — Every discovery documented chronologically
- ⚔ **Community Submissions** — Submit your own findings via form

## How to Update

### Adding New Audio Files
1. Place WAV files in the correct subfolder under `audio/`
2. Update `assets/js/tracks.js` with new track entries
3. Commit and push — GitHub Pages auto-deploys

### Adding Research Log Entries
Edit `pages/research.html` — add a new `.entry` div at the top of the timeline

### Adding Format Documentation
Edit `pages/formats.html` — add a new tab panel

### Activating the Submit Form
1. Go to [formspree.io](https://formspree.io) and create a free form
2. Replace `YOUR_FORM_ID` in `pages/submit.html` with your form ID

## GitHub Pages Setup

1. Push this repo to GitHub: `git remote add origin https://github.com/YOUR_USERNAME/mkshaolinmonks.git`
2. Go to repo Settings → Pages → Source: Deploy from branch → main → / (root)
3. Site will be live at `https://YOUR_USERNAME.github.io/mkshaolinmonks`

> **Note:** Audio files (180MB+) are stored in `audio/` — you may want to use Git LFS or host audio on a CDN and update the paths in `tracks.js`

## Key Discoveries

| Discovery | Status |
|-----------|--------|
| Engine name: **Paradox Engine** | ✅ Confirmed |
| Project codename: **Mka** | ✅ Confirmed |
| 103 audio tracks decoded | ✅ Complete |
| Full middleware stack (CRI, Havok, Flash) | ✅ Confirmed |
| 7,139 WAD entries mapped | ✅ Confirmed |
| PWF entry table stride | ⚠️ In Progress |
| EWDF chunk type IDs | ⚠️ In Progress |
| Hidden WAD: GAMEDATA.WAK | ❓ Mystery |
| Textures extracted | ❌ Pending |
| 3D models extracted | ❌ Pending |

## File Structure

```
mkshaolinmonks/
├── index.html              # Homepage
├── assets/
│   └── css/mk.css         # Shared styles
├── pages/
│   ├── audio.html         # Audio player (103 tracks)
│   ├── formats.html       # File format docs
│   ├── assets.html        # Assets gallery
│   ├── research.html      # Research log
│   ├── submit.html        # Community submission form
│   └── about.html         # About OGmidway
└── audio/                 # WAV audio files (host separately or Git LFS)
```
