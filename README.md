# YT Fast Scraper 🚀

A highly optimized, serverless, and client-side YouTube Data API v3 scraper. Designed specifically to bypass mobile lite-browser limitations, this tool allows for unhindered scraping, intelligent querying, and direct YouTube account management without leaving the page.

## ✨ Core Features

### 🔍 Advanced Search & Scraping
* **Universal Input:** The search box automatically detects regular keywords, direct Video URLs, direct Playlist URLs, and Channel IDs.
* **Smart `@handle` Detection:** Typing `@handle` instantly shifts the API into Channel Search mode.
* **"No Limits" Deep Scraping:** While standard searches obey the UI limits (25/50/100/250) to protect browser memory, scraping a specific Channel or Playlist via the menu automatically paginates through Google's API to fetch *every single video* (e.g., pulling 1,000+ videos silently in the background).
* **Trending & Popular:** Access Google's raw `mostPopular` charts. Select a specific category (Gaming, News, Music) to pull the top trending videos in your country.
* **View-Count Sorting:** Typing a keyword while in "Popular" mode automatically shifts the API to scrape the most-viewed videos in YouTube history for that term.

### 📦 Download Queue & Export
* **Smart Queue System:** Select specific videos and drop them into a holding queue. The queue automatically strips out duplicate URLs.
* **Lite Browser "Share" Bypass:** Built specifically for strict mobile browsers (Via, X Browser). If the native Web Share API is blocked, the app forces a text-highlight overlay so the Android OS universal Share popup appears natively.
* **1-Click Copy:** Copy thousands of scraped URLs to your clipboard instantly.

### 🔐 OAuth & Account Actions
* **Zero-Footprint Searching:** All searches are executed via the API, meaning your queries will **never** affect your YouTube recommendations or appear in your YouTube search history.
* **Get Subscriptions:** One-click fetch to see the latest uploads from channels you are subscribed to.
* **Secret Playlist Creation:** Inject your entire scraped queue directly into a new Private Playlist on your YouTube channel automatically. 

### ⚙️ UI & Quality of Life
* **State-Aware Bookmarks (⭐):** The bookmark button doesn't just save your search term; it perfectly memorizes your exact API Type and Category dropdown states.
* **Infinite Pagination:** A dynamic "Load More Results" button remembers your exact API `pageToken`, allowing you to scroll through databases infinitely.
* **Localized Status Messages:** No more jumping to the top of the page to read errors. Success/Error messages appear explicitly beneath the specific button you clicked.
* **Floating Navigation:** Non-intrusive ▲ and ▼ arrows to instantly jump to the top or bottom of massive scraping lists.
* **App Generator:** Compile all your API keys and UI preferences into a standalone, hardcoded HTML file with one click.

### 🌍 Localization
* **Dynamic Region Swapping:** Instantly change the global API region code to pull trending data from specific countries (defaults to 🇪🇬 EG). 
* **Optimized Arabic Layout:** Video title areas are widened and dynamically spaced to prevent Arabic characters from overlapping with UI badges.
