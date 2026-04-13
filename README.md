# 🎬 AI for Kids — Video Generation Prompt

A cinematic JSON-based prompt script designed for AI video generation tools. The prompt brings to life an inspiring short film featuring an Indian school boy discovering AI through the **SocialEagle AI Platform** — from confusion at homework to confidently using AI and teaching his friends.

---

## ⚠️ Git LFS Required — Install Before Cloning

This repository contains large video files (`.mp4`) tracked using **Git Large File Storage (LFS)**.  
**You must install Git LFS before cloning**, otherwise the video file will not download correctly.

### 1. Install Git LFS

#### Windows
```bash
# Using winget
winget install GitHub.GitLFS

# Or download the installer from:
# https://git-lfs.com
```

#### macOS
```bash
brew install git-lfs
```

#### Linux (Debian/Ubuntu)
```bash
sudo apt install git-lfs
```

### 2. Activate Git LFS (run once after install)
```bash
git lfs install
```

### 3. Clone the Repository
```bash
git clone <your-repo-url>
```

> **Note:** If you already cloned without LFS installed, run `git lfs pull` inside the repo to fetch the large files.

---

## 📁 Project Structure

```
JSON_Prompt_Video_AI_FOR_KIDS/
├── prompt.txt          # JSON scene-by-scene video generation prompt
├── Prompt Battle.mp4   # Final rendered AI-generated video (tracked via Git LFS)
├── .gitattributes      # Git LFS tracking rules (*.mp4)
└── README.md
```

---

## 🎥 Video Prompt Overview

The `prompt.txt` file contains a structured JSON prompt with **9 scenes** spanning **~30 seconds**:

| Scene | Duration | Description |
|-------|----------|-------------|
| 1 | 0–5s | Boy struggling with homework at his study table |
| 2 | 5–8s | Close-up of crossed-out math problems and frustration |
| 3 | 8–12s | A mysterious paper note drifts in: *"Learn AI, Build Anything"* |
| 4 | 12–16s | Boy opens laptop, discovers SocialEagle AI Platform |
| 5 | 16–20s | AI explains math step-by-step; boy's face lights up |
| 6 | 20–23s | Boy confidently explores AI tools with diagrams and notes |
| 7 | 23–26s | Boy teaches classmates using laptop in collaborative setting |
| 8 | 26–28s | Boy builds a mobile app using AI tools |
| 9 | 28–30s | Hero shot: *"Learn AI with Social Eagle and start flying"* |

---

## 🛠️ Prompt Format

Each scene follows this JSON structure:

```json
{
  "scene": 1,
  "duration": "0-5s",
  "style": "ultra-realistic cinematic, natural lighting, 4K",
  "character": "A Indian school boy (10-12 yrs, light blue uniform...)",
  "camera": "slow push-in, eye-level, shallow depth of field",
  "prompt": "Detailed visual description for the AI video model..."
}
```

### Fields

| Field | Description |
|-------|-------------|
| `scene` | Scene number |
| `duration` | Timestamp range in seconds |
| `style` | Cinematic style and rendering quality |
| `character` | Character description (kept consistent across scenes) |
| `camera` | Camera movement and framing |
| `prompt` | Full descriptive prompt for the AI video generator |

---

## 🚀 How to Use

1. Copy individual scene JSON blocks from `prompt.txt`.
2. Paste into your preferred AI video generation tool (Kling, Pika, Runway, etc.).
3. Generate each scene separately and stitch together in a video editor.

---

## 📌 Notes

- The character design is kept **consistent across all scenes** using the same description.
- Lighting evolves naturally from **dim and warm** (confusion) → **bright and cool** (confidence).
- The closing scene is designed as a **hero/brand shot** for SocialEagle AI.
