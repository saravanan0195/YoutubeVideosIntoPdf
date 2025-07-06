# 🎞️ YouTube Videos into PDF

**YouTube Videos into PDF** is a Python-based automation tool that converts YouTube videos—including Shorts and Playlists—into high-quality PDF documents. It extracts unique frames from videos using structural similarity metrics and overlays accurate timestamps for easy reference. Perfect for students, researchers, educators, or content archivists who want to preserve visual content offline.

--

## 🚀 Features

- ✅ Supports standard YouTube videos, Shorts, and Playlists
- 🧠 Uses Structural Similarity Index (SSIM) to detect unique frames
- 🕒 Embeds timestamp overlays on each frame
- 📄 Converts images into a clean, scrollable landscape PDF
- 🎨 Dynamic text color detection (white/black) for clear visibility
- 📥 Auto-download of PDF upon completion (for Google Colab users)

---

## 🛠️ Tech Stack

- `Python 3.x`
- [`yt-dlp`](https://github.com/yt-dlp/yt-dlp) – YouTube video downloader
- `OpenCV` – Frame capture and image processing
- `scikit-image` – Structural similarity computation
- `Pillow (PIL)` – Image manipulation
- `FPDF` – PDF generation
- `Google Colab` – Optional environment for seamless execution

---

⚙️ Workflow

Step-by-Step Process:

Input: The user enters a YouTube video, Shorts, or Playlist URL.

Download: The video is downloaded using yt-dlp.

Frame Extraction: Frames are extracted and compared using SSIM.

Filtering: Visually similar frames are discarded to keep only unique shots.

Timestamping: Each unique frame gets a timestamp (HH:MM:SS).

Color Logic: Text color is adjusted based on brightness (white or black).

PDF Generation: All selected frames are compiled into a landscape-oriented PDF using fpdf.

Download Output: The final PDF is saved or auto-downloaded.


## 📦 Installation

Run the following commands in your environment or in a Google Colab notebook:

```bash
pip install opencv-python-headless
pip install scikit-image
pip install fpdf
pip install yt-dlp
---




