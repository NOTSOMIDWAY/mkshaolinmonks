# MK Shaolin Monks Research Archive

**Created by OGmidway** | [Live Site](https://ogmidway.github.io/mkshaolinmonks)

The first publicly documented reverse-engineering archive for **Mortal Kombat: Shaolin Monks (2005)**, built on the **Paradox Engine** by Midway Studios LA.

## What's Here

- 🔊 **Audio Player** — 103 decoded ADX audio files from GAMEDATA.WAI
- 📂 **File Formats** — PWF, EWDF, CRI AFS, CRI ADX, ps2_DTPK documented
- 🖼 **Assets Gallery** — All extracted game assets
- 📜 **Research Log** — Every discovery documented chronologically
- ⚔ **Community Submissions** — Submit your own findings via form

> **Note:** Audio files (180MB+) are stored in `audio/`

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
