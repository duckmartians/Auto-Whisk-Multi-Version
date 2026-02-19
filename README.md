<p align="center">
  <img width="100" height="100" alt="logo" src="https://github.com/user-attachments/assets/86f005b2-bc0c-4542-bd70-3d556a4ff8ce" />
</p>

<h1 align="center">Auto Whisk</h1>
<p align="center">
  Batch AI image generation with Google Whisk — fully automated.<br>
  Version 8.3.0 · 7 languages · by <a href="https://duckmartians.info">duckmartians</a><br><br>
  <a href="https://github.com/duckmartians/G-Labs-Automation/releases/latest"><img src="https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge" alt="Download Here"></a><br><br>
  <a href="README.md"><img src="https://img.shields.io/badge/English-blue" alt="English"></a>
  <a href="README_vi.md"><img src="https://img.shields.io/badge/Tiếng%20Việt-green" alt="Tiếng Việt"></a>
</p>

---

## 📖 What is Auto Whisk?

A Chrome extension that **automatically generates images in bulk** on [Google Whisk AI](https://labs.google/fx/tools/whisk). Instead of typing prompts one by one:

- Enter a **list of prompts** → Extension generates images sequentially  
- Enable **auto-download** → Images are saved as soon as they're ready  
- **Pause / Resume / Stop** at any time  
- **Retry** failed images with a single click  

> The extension opens as a **side panel** — it doesn't cover your main screen.

---

## 🚀 Mode Selection Screen (Gateway)

Click the extension icon → the side panel shows 3 options:

| | Mode | Description |
|:---:|---|---|
| 🟢 | **7.6.0 — Fast** (Recommended) | Runs in background, no need to open Whisk. Full features. |
| ⚪ | **7.5.1 — Classic** (Fallback) | Simulates mouse on Whisk page. Use when Fast mode fails. |
| 🟣 | **G-Labs Automation** | Standalone Windows software, no browser needed. |

🌐 Top-right corner has a **language selector** (7 languages) — your choice is saved automatically.

---

## ⚡ Fast Mode (7.6.0)

> **Recommended** — High speed, stable background execution, no need to open Whisk.

### Entering Prompts

Type/paste prompts into the text box, or click **"Import from file"** to load a `.txt` file.

**Two prompt-splitting modes:**

| Mode | How it works | When to use |
|---|---|---|
| **1 line = 1 prompt** | Each line is treated as a separate prompt | Short prompts |
| **Blank line separated** | Consecutive lines are merged into 1 prompt | Long multi-line prompts |

### Settings

| Option | Details |
|---|---|
| **Aspect Ratio** | [1:1](file:///d:/Data/Downloads/8.2.2_0/v7.5.1/i18n.js#456-463) · `16:9` · `9:16` · `4:3` · `3:4` |
| **Image Count** | 1 → 4 images (e.g. 10 prompts × 3 images = 30 images) |
| **Save Folder** | Subfolder name inside Downloads |
| **Auto-download** | On/off — default **on** |

### 🎨 Reference Images

Attach sample images so the AI mimics a specific style, subject, or scene.

Click **"Reference Images"** → a management panel opens:

| Category | Description | Max |
|---|---|:---:|
| **Subject** | Character / object you want the AI to recreate | 2 |
| **Scene** | Background / environment to place the subject in | 1 |
| **Style** | Artistic style you want the AI to follow | 1 |

**How to use:** Click `+` to select an image → Click **"Upload & Analyze"** → Edit caption if needed → **"Save Caption"** → **"Done"**.

> Reference images apply to **all** prompts in your list.

### Controls

| Button | Function |
|:---:|---|
| ▶ **Start** | Begin generating images sequentially |
| ⏸ **Pause** | Click again to resume |
| ⏹ **Stop** | Stop the entire process |

### Results Table

| Column | Meaning |
|---|---|
| **#** | Row number |
| **Prompt** | Prompt text *(editable directly)* |
| **IMG 1, 2…** | Thumbnail — click to **view full size** |
| **Status** | ⏳ Pending · 🔄 Generating · ✅ Done · 🔃 Error *(click to retry)* |

If any row fails → a **"Retry All Errors"** button appears to retry all at once.

### Authentication

The extension **automatically retrieves your Google session**. If no `labs.google` tab is open, it opens a hidden tab → waits for you to sign in → saves the session automatically. Expired sessions are **refreshed automatically**.

> ⚠️ You need a Google account with access to Google Labs.

---

## 🖱️ Classic Mode (7.5.1)

> **Fallback** — Simulates mouse actions on the Whisk page. Requires the Whisk tab to stay open.

### Requirements

- The Whisk tab must be **open** and **active** (in focus)  
- The extension automatically zooms the page to 50% for optimization  

### Two Start Options

| Option | Description |
|---|---|
| 🚀 **Create New Project** | Opens Whisk, creates a new project, then starts |
| ➡️ **Run on This Project** | Runs immediately on the already-open project |

### Additional Settings

| Option | Details |
|---|---|
| **Wait time** | Random (min–max seconds) or fixed (≥10 seconds) |
| **Runs per prompt** | Each round Whisk creates 2 images (e.g. 5 prompts × 3 repeats = 30 images) |
| **Start from prompt** | Enter a number to skip earlier prompts |

### Logs & Error Handling

- 📋 **Detailed Log** — tracks every step: preparation, sending, downloading, errors…  
- 📝 **Failed Prompts** — listed with reasons, click **"Copy Failed Prompts"** to copy and retry  
- 🔄 **Auto-retry** when queue is full (up to 20 attempts + page reload)  
- ⏳ **Auto-wait** when an error toast appears, resumes when it clears  
- 📥 **Final sweep scan** (30 seconds) to ensure no images are missed  

---

## 📊 Mode Comparison

| Feature | ⚡ 7.6.0 Fast | 🖱️ 7.5.1 Classic |
|---|:---:|:---:|
| Requires Whisk tab | ❌ | ✅ Required |
| Speed | ⚡ Fast | 🐢 Slower |
| Stable background run | ✅ | ⚠️ Needs tab |
| Image Count / prompt | 1–4 custom | Fixed 2 |
| Reference images | ✅ | ❌ |
| Filename by content | ✅ | Sequential number |
| Aspect Ratio options | 5 ratios | Whisk default |
| Multi-line prompts | ✅ | ❌ |
| Custom wait time | Auto 2–5s | ✅ Custom |
| Runs per prompt | Use Image Count | ✅ Custom |
| Detailed Log | Brief status | ✅ Full log |
| Zoom image preview | ✅ | ❌ |
| Edit prompt in table | ✅ | ❌ |

---

## 💡 Tips

- **Disable "Ask where to save..."** in your browser's download settings for uninterrupted auto-downloads  
- All settings are **auto-saved** — reopening the extension restores your last session  
- Click 🏠 in the top-left corner to return to the **mode selection screen** at any time  

---

<p align="center">
  <b>Designed by <a href="https://duckmartians.info">duckmartians</a></b><br>
  <a href="https://discord.gg/munMZEBMw5">Discord</a> ·
  <a href="https://github.com/duckmartians/Auto-Whisk-Multi-Version">GitHub</a>
</p>
