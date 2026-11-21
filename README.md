# UPSCALER BY VENOZK

**Free, private, client-side AI Image & Video Upscaler + Background Remover**

A single-file HTML web app that runs 100% in the browser. No server, no uploads, no accounts, no watermarks.

## Features

| Feature | Model / Tech | Notes |
|---------|--------------|-------|
| **Image Upscale** (2× / 4×) | UpscalerJS + ESRGAN (TensorFlow.js) | Super-resolution |
| **Image Background Removal** | `@imgly/background-removal` (ISNet) | High quality transparent PNG |
| **Combined** | Upscale then Remove BG | One-click pipeline |
| **Video Background Removal** | MediaPipe Selfie Segmentation | Best for people / portraits |
| **Video Export** | Canvas + MediaRecorder | Transparent WebM |

## How to use

1. Open `index.html` in a modern browser (Chrome / Edge recommended).
2. Or upload the whole folder to **GitHub Pages**.

### Image
- Drop or select an image
- Choose 2× or 4×
- Click **AI Upscale**, **Remove Background**, or **Upscale + Remove BG**
- Download the result

### Video
- Drop a short video (people / faces work best)
- Click **Remove Background** for a preview frame
- Click **Process & Export WebM** to render the full clip
- Download

## Important notes

- **First run** downloads AI models (30–80 MB). They are cached by the browser.
- Everything stays on the user’s device — perfect for private photos.
- Video processing is CPU/GPU intensive. Keep clips short (≤15–20 s) for best experience.
- Full long-form AI video upscaling is still too heavy for pure browser use. Use this tool for BG removal, then a desktop upscaler (Upscayl, Video2X, Topaz, etc.) if needed.

## Tech stack

- Vanilla HTML + CSS + JS
- TensorFlow.js + UpscalerJS
- @imgly/background-removal
- MediaPipe Selfie Segmentation
- No build step required

## Deploy to GitHub Pages

1. Create a new repository
2. Upload `index.html` (and this README)
3. Settings → Pages → Deploy from main branch
4. Done. Your tool is live.

---

**UPSCALER BY VENOZK** — Built for privacy and free forever.
