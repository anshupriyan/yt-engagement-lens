# 👎 YT Dislike Preview

A lightweight, Manifest V3 Chrome Extension that brings back YouTube dislike counts directly on thumbnails, watch pages, and YouTube Shorts — **no API key required.**

## ✨ Features

*   **Thumbnail Overlays:** View like and dislike counts inline as native-looking metadata on the home feed, search results, sidebar recommendations, channel pages, and playlist grids.
*   **Watch Page Metrics:** Displays exact dislike counts directly below the main video description area.
*   **YouTube Shorts Integration:** Restores dislike counts on the YouTube Shorts sidebar action buttons.
*   **Zero Configuration:** Works out-of-the-box using the public Return YouTube Dislike API, without requiring personal API keys.
*   **Lightweight & Fast:** Built entirely with vanilla JavaScript and CSS to minimize browser memory footprint.

## 🛠️ Installation (Developer Mode)

Since this extension is loaded locally for development:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/anshupriyan/yt-engagement-lens.git
    ```
2.  Open Google Chrome and navigate to `chrome://extensions/`.
3.  Enable **Developer mode** (toggle in the top-right corner).
4.  Click **Load unpacked** in the top-left corner.
5.  Select the project root folder (containing the `manifest.json` file).

## ⚙️ How It Works

The extension injects a content script (`content.js`) onto YouTube pages that dynamically scans for video elements and sidebar elements. It then fetches historical dislike data from the public Return YouTube Dislike API using a background service worker (`background.js`) to bypass CORS restrictions, caching the data in memory to ensure fast and efficient rendering.

## 📊 Attribution & Data Source

This project retrieves its data from the public API provided by [Return YouTube Dislike](https://returnyoutubedislike.com/). We attribute and thank the Return YouTube Dislike project and its contributors for their excellent work and for making this data available. 

*   **Website:** [returnyoutubedislike.com](https://returnyoutubedislike.com/)
*   **Source Code:** [Anarios/return-youtube-dislike on GitHub](https://github.com/Anarios/return-youtube-dislike)

## 🛡️ License

Distributed under the MIT License. See `LICENSE` for more details.
