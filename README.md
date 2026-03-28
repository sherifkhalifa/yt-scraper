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
* *Security Tip:* Once you generate your final private Netlify link in Step 3, come back here, click your key, select **Websites**, and add your Netlify link to protect your quota.

**2. The OAuth Client ID (Optional, for Private Playlists):**
* On the [Credentials Page](https://console.cloud.google.com/apis/credentials), click **+ CREATE CREDENTIALS** -> **OAuth client ID**.
* Select **Web application**. 
* Under **Authorized JavaScript origins**, click **+ ADD URI**. You will paste your final Netlify link here in Step 3.

---

## 📥 Step 2: Generate Your Private App
Now that you have your keys, you can generate your clean, standalone HTML file.

1. Open the [Public Generator Link](https://sherifkhalifa.github.io/yt-scraper/).
2. Scroll to the bottom and open **"⚙️ App Setup & Keys"**.
3. Paste your API Key and Client ID into the boxes.
4. *(Optional)* Type your email in the Reminder Box so the app reminds you which Google account to log in with later.
5. Click **Download Clean App**.
6. A file named `YT_Clean_App.html` will download to your device. **This file contains your private keys. Do not upload this specific file back to your public GitHub.**

---

## 🌐 Step 3: Host Securely via Private GitHub & Netlify Sync
To use your new app safely, you will store the code in a *Private* GitHub repository and use Netlify to host it. This gives you a completely anonymous link and automatically updates your app if you ever edit the code.

### A. Create a Secret GitHub Repository
1. Go to your GitHub account and click **+ New Repository**.
2. Name it something random (e.g., `my-private-scraper`).
3. **CRITICAL:** Select **Private** (so no one on the internet can see your keys).
4. Click **Create repository**.
5. Click **"uploading an existing file"** and upload the `YT_Clean_App.html` file you just generated.
6. **Rename the file:** Once uploaded, edit the file name and change it from `YT_Clean_App.html` to `index.html`. Commit the changes.

### B. Sync to Netlify for an Anonymous Link
1. Go to [Netlify.com](https://www.netlify.com/) and log in using your GitHub account.
2. In the dashboard, click **Add new site** -> **Import an existing project**.
3. Click the **GitHub** button to authorize the connection.
4. Select your newly created private repository (`my-private-scraper`).
5. Scroll to the bottom and click **Deploy site**.
6. Netlify will instantly generate a live, anonymous link (e.g., `https://happy-frog-1234.netlify.app`). You can go to Site Settings to change this name to whatever you want.

### C. Final Security Check
Now that you have your permanent Netlify link, go back to your [Google Cloud Credentials](https://console.cloud.google.com/apis/credentials):
* Add the Netlify link to your **OAuth Client ID** "Authorized JavaScript origins" so the login button works.
* Add the Netlify link to your **API Key** "Website restrictions" so no one else can steal your quota.

You can now bookmark your Netlify link on your phone. It is 100% private, anonymous, and requires zero setup to use!
