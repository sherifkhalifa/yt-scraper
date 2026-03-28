# YT Fast Scraper & Generator

A lightning-fast, client-side YouTube scraping tool that bypasses public rate limits by utilizing your own official Google API keys. 

**Public App & Generator Link:** 👉 [https://sherifkhalifa.github.io/yt-scraper/](https://sherifkhalifa.github.io/yt-scraper/)

---

## 🛠️ How this Tool Works
Because public YouTube scrapers often hang or fail due to server blocks, this HTML app connects directly to Google's official backend. 

The live link above acts as a **Generator**. You can use it to test searches, but its main purpose is to build a completely private, standalone web app for yourself. By entering your API keys and clicking "Download Clean App," the generator injects your keys invisibly into the code and strips away all setup menus, giving you a pure, zero-step scraping tool.

---

## 🚀 Step 1: Get Your Free Google Keys
To prevent errors and throttling, you need your own free Google credentials.

**1. The API Key (Required for Searching):**
* Go to the [Google Cloud API Library](https://console.cloud.google.com/apis/library/youtube.googleapis.com) and click **Enable**.
* Go to the [Credentials Page](https://console.cloud.google.com/apis/credentials), click **+ CREATE CREDENTIALS**, and select **API Key**.
* *Security Tip:* Click on your new key, select **Websites** under Application restrictions, and add `*sherifkhalifa.github.io/*` so no one else can use it.

**2. The OAuth Client ID (Optional, for Private Playlists):**
* On the [Credentials Page](https://console.cloud.google.com/apis/credentials), click **+ CREATE CREDENTIALS** -> **OAuth client ID**.
* Select **Web application**. 
* Under **Authorized JavaScript origins**, click **+ ADD URI** and paste `https://sherifkhalifa.github.io`.

---

## 📥 Step 2: Generate Your Private App
Now that you have your keys, you can generate your clean, standalone HTML file.

1. Open the [Public Generator Link](https://sherifkhalifa.github.io/yt-scraper/).
2. Scroll to the bottom and open **"⚙️ App Setup & Keys"**.
3. Paste your API Key and Client ID into the boxes.
4. *(Optional)* Type your email in the Reminder Box so the app reminds you which Google account to log in with later.
5. Click **Download Clean App**.
6. A file named `YT_Clean_App.html` will download to your device. **This file contains your private keys. Do not upload this specific file back to a public GitHub.**

---

## 🌐 Step 3: Host Your Private App Anonymously (Netlify)
To use your new `YT_Clean_App.html` file like a real mobile app without exposing your code or real name to the public, host it for free on Netlify.

1. Go to [Netlify Drop](https://app.netlify.com/drop) on your browser (you may need to create a free account).
2. Simply upload/drop your downloaded `YT_Clean_App.html` file into the upload box.
3. Netlify will instantly create a live, anonymous website (e.g., `https://happy-frog-1234.netlify.app`). 
4. **Important:** If you used an OAuth Client ID for logins, you must go back to your Google Cloud Credentials page and add your new Netlify link to the "Authorized JavaScript origins" list, just like you did for the GitHub link.

You can now bookmark your Netlify link on your phone's home screen. Whenever you open it, the app will instantly unlock using your hidden keys with zero setup required.

