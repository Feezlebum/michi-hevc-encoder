# HEVC with Alpha Encoder

This GitHub Action encodes PNG frames into HEVC video with alpha transparency for iOS apps.

## Setup

1. Create a new GitHub repository
2. Copy the `.github/workflows/encode-hevc-alpha.yml` file to your repo
3. Create a `frames/` folder and upload your PNG frames (named `frame_0001.png`, `frame_0002.png`, etc.)
4. Go to **Actions** tab → **Encode HEVC with Alpha** → **Run workflow**
5. Wait ~2 minutes, then download `hevc-alpha-video` artifact

## Customization

Edit the workflow to change:
- `-framerate 24` — change FPS
- `-alpha_quality 0.75` — quality 0-1 (higher = better but bigger)
- Input pattern if your frames are named differently
