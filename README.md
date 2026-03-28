# YT Fast Scraper & Generator

A lightning-fast, client-side YouTube scraping tool that bypasses public rate limits by utilizing your official Google API keys. 

**How to start:** Simply host the `index.html` file on any web server or free hosting platform (like GitHub Pages or Netlify) and open the link in your browser. The app will automatically detect its own web address and guide you through the setup.

---

## 🛠️ How this Tool Works
Because public YouTube scrapers often hang or fail due to server blocks, this HTML app connects directly to Google's official backend. 

The `index.html` file acts as a **Generator**. You can use it to test searches, but its main purpose is to build a completely private, standalone web app for yourself. By entering your Google keys and clicking "Download Clean App," the generator injects your keys invisibly into the code and strips away all setup menus, giving you a pure, zero-step scraping tool. 

*(Note: The generated private app will always contain a subtle backdoor link at the bottom to return to your original generator if you ever need to rebuild it).*

---

## 🚀 Step 1: Get Your Free Google Keys
To prevent errors and throttling, you need your own free Google credentials. The app will physically show you the exact web address you need to whitelist in the instructions on your screen.

**1. The API Key (Required for Searching):**
* Go to the [Google Cloud API Library](https://console.cloud.google.com/apis/library/youtube.googleapis.com) and click **Enable**.
* Go to the [Credentials Page](https://console.cloud.google.com/apis/credentials), click **+ CREATE CREDENTIALS**, and select **API Key**.
* *Restriction (OPTIONAL):* You can leave this unrestricted to work anywhere. However, to protect your quota from theft, you should eventually edit the key, select **Websites**, and paste the URL that the app tells you to use.

**2. The OAuth Client ID (Optional, for Private Playlists):**
* On the [Credentials Page](https://console.cloud.google.com/apis/credentials), click **+ CREATE CREDENTIALS** -> **OAuth client ID**.
* Select **Web application**. 
* *Restriction (MANDATORY):* Under **Authorized JavaScript origins**, you MUST click **+ ADD URI** and paste the exact URL displayed in the app's setup box.

---

## 📥 Step 2: Generate Your Private App
Now that you have your keys, you can generate your clean, standalone HTML file.

1. Open your hosted generator link.
2. Scroll to the bottom and open **"⚙️ App Setup & Keys"**.
3. Paste your API Key and Client ID into the boxes.
4. *(Optional)* Type your email in the Reminder Box so the app reminds you which Google account to log in with later.
5. Click **Download Clean App**. Accept the pop-up warning.
6. A file named `YT_Clean.html` will download to your device. **This file contains your private keys. Do not upload this specific file back to a public repository.**

---

## 🌐 Step 3: Host Your Private App Anonymously
To use your new `YT_Clean.html` file safely as a mobile web app, you should host it on Netlify. Choose one of the two methods below.

### Method A: The Quick Way (Netlify Drop - No GitHub Required)
Use this method if you just want to drag and drop the file and be done in 10 seconds.
1. Go to [Netlify Drop](https://app.netlify.com/drop) on your browser.
2. Upload or drag your downloaded `YT_Clean.html` file into the upload box.
3. Netlify will instantly create a live, anonymous website (e.g., `https://happy-frog-1234.netlify.app`).

### Method B: The Automated Way (Private GitHub Repo + Netlify Sync)
Use this method if you want to store your private code safely in the cloud and allow automatic updates.
1. Go to your GitHub account and create a **+ New Repository**. 
2. **CRITICAL:** Select **Private** (so no one on the internet can see your keys). Click Create.
3. Upload the `YT_Clean.html` file you just generated to this new repository, and rename the file to `index.html`.
4. Go to [Netlify.com](https://www.netlify.com/) and click **Add new site** -> **Import an existing project**.
5. Click **GitHub**, select your private repository, and click **Deploy site**.
6. Netlify will instantly generate a live, anonymous link.

---

### 🔒 Step 4: Final Security Check (CRITICAL)
When you host your private app on Netlify, **your web URL changes**. If you try to log in immediately, Google will block you because it doesn't recognize the new Netlify address.

1. Open your new Netlify link on your phone.
2. Scroll to the very bottom. The app will auto-detect its new home and say: `Running on: https://your-new-site.netlify.app`.
3. Copy that exact URL.
4. Go back to your [Google Cloud Credentials](https://console.cloud.google.com/apis/credentials).
5. Edit your **OAuth Client ID** and add the Netlify link to "Authorized JavaScript origins".
6. *(Optional)* Edit your **API Key** and add the Netlify link to "Website restrictions".

Your private scraper is now 100% secure, fully functional, and ready to use!
