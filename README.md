# C1 Offers Sorter

> Search, sort, and organize Capital One Shopping offers by mileage value with natural, human-like pacing for reliable loading.

---

## ⚡ What's New in this Version

- **Human-Like Pacing**: Includes randomized pauses (1 to 5 seconds) between "View More Offers" clicks, simulating natural human browsing behavior and preventing request throttling so all offers load smoothly.
- **Enhanced Reliability**: Automatically monitors response statuses and backs off gracefully if rate limits are reached.

---

## 🚀 How to Install in Google Chrome

Choose either **Method 1 (Easiest - No Node.js required)** or **Method 2 (Build from Source)**.

### Method 1: Using Pre-built Zip (Recommended & Quickest)

1. **Download the Extension:**
   - Go to the [Releases](https://github.com/matteoago/C1/releases) page.
   - Download the latest `c1-offers-sorter-chrome.zip`.
2. **Unzip the File:**
   - Extract `c1-offers-sorter-chrome.zip` to a folder on your computer (e.g. into your `Downloads` or `Documents` folder).
3. **Load in Chrome:**
   - Open Google Chrome and type `chrome://extensions` in the address bar (or go to `Menu (⋮)` > `Extensions` > `Manage Extensions`).
   - Turn **ON** the **Developer mode** toggle in the top-right corner.
   - Click the **Load unpacked** button in the top-left corner.
   - Select the unzipped folder (the folder containing `manifest.json`).
4. **Done!** The extension icon will now appear in your Chrome toolbar.

---

### Method 2: Build from Source

If you have Node.js installed and want to build the extension yourself:

```bash
# 1. Clone the repository
git clone https://github.com/matteoago/C1.git
cd C1

# 2. Install dependencies
npm install

# 3. Build the extension for Chrome
npm run build
```

Then load it into Chrome:
1. Open Chrome and navigate to `chrome://extensions`.
2. Toggle on **Developer mode** (top right).
3. Click **Load unpacked** (top left).
4. Select the `dist/chrome-mv3` folder inside the `C1` directory.

---

## 📖 How to Use

1. **Navigate to Capital One Offers:**
   - Visit [capitaloneoffers.com/feed](https://capitaloneoffers.com/feed) or [capitaloneoffers.com/c1-offers](https://capitaloneoffers.com/c1-offers) and log in.
2. **Open the Extension:**
   - Click the **C1 Offers Sorter** icon in your Chrome toolbar. (Tip: Click the puzzle piece icon to pin it to your toolbar).
3. **Sort Your Offers:**
   - Choose your sort criteria (**Mileage** or **Alphabetical**).
   - Select the order (**Highest to Lowest** or **Lowest to Highest**).
   - Click **"Load & Sort Offers"**.
   - The extension will automatically paginate through the offers with random 1–5 second pauses to ensure steady, uninterrupted loading.
4. **Search Across All Offers:**
   - Use the built-in instant search box to quickly filter by merchant name (supports fuzzy matching for typos).
5. **Manage Favorites:**
   - Enable the Favorites toggle to star deals you want to save for later.
   - Click "Show Favorites Only" to view just your saved offers.

---

## 🔒 Security & Privacy

- **100% Local**: All sorting, searching, and favorites are handled strictly inside your browser. No data, credentials, or cookies are ever transmitted to any third-party server.
- **Minimal Permissions**: Uses only `activeTab`, `scripting`, and `storage` (to save your favorite stars locally).
- **Open Source**: The code is completely open and inspectable.

---

## 📄 License

This project is licensed under the MIT License.

*Disclaimer: This extension is an independent tool and is not affiliated with, sponsored by, or endorsed by Capital One.*
