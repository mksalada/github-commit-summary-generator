# Changelog

All notable changes to GitSum are documented here.

---

## [v1.4.0] - 2026-03-25
### 🎨 UI & Layout
- Restored **subtitle** under the title “GitSum”  
- Restored **footer** with credit  
- Light/Dark theme toggle button  
- Branch dropdown auto-loads all available branches  

### ⚡ Refactor & Structure
- Fully refactored JavaScript into modules:
  - `api.js` – GitHub API calls and error handling  
  - `ui.js` – DOM updates for loading, errors, and output  
  - `formatter.js` – Format commit data (Markdown, JSON, Text)  
  - `main.js` – Controller logic  

### ✅ Bug Fixes
- Downloads now correctly produce `.md`, `.txt`, or `.json` files  
- Proper error messages for invalid repository input  
- Fixed branch selection issues during commit summary generation  
- Rate limit alert updates dynamically and visually stands out  

### 🌿 Accessibility & UX
- Skip link for screen readers  
- `aria-label`s for inputs and dropdowns  
- `aria-live="polite"` for the output panel  
- Output panel scrollable and readable on all screen sizes  

### 💡 Notes
- Focused on **stability, usability, and maintainability**  
- Fully compatible with GitHub Pages deployment  
- No new features added—improvements are mostly behind-the-scenes

---

## [v1.3.0] - 2026-03-25
### 🎨 UI/UX Improvements
- Redesigned interface with modern card layout  
- Added light/dark mode toggle (with saved preference)  
- Improved spacing, typography, and input grouping  
- Smaller, cleaner theme toggle button  

### 🌿 Smarter Repository Handling
- Auto-detects repository default branch  
- Dynamically loads and displays all available branches  
- Prevents invalid branch selection via dropdown  

### 📦 Multi-Format Export
- Export commit summaries as Markdown (`.md`), JSON (`.json`), Plain Text (`.txt`)  
- Smart file naming based on repository  

### 🚦 API Awareness
- Added GitHub API rate limit indicator  
- Displays remaining requests in real-time  
- Warns when nearing limit  
- Clarifies usage of unauthenticated (public) API  

### ✅ Validation & Error Handling
- Improved repository format validation ("owner/repo")  
- Clearer error messages for invalid repos, missing commits, and API rate limits  

### ⚡ Performance & Structure
- Refactored code into data normalization, formatting, fetch logic  
- Improved pagination handling  

### 💡 Notes
- Uses public GitHub API (no authentication, 60 requests/hour)  

---

## [v1.2.0] - 2026-03-25
### ✨ New Features
- Export generated summaries in multiple formats: `.json`, `.md`, `.txt`  
- One-click export from interface  

### 🎉 Improvements
- Refactored scripts to support file generation and downloads  
- Updated UI elements (title, buttons, structure)  
- Improved usability and interaction flow  

### ✅ Stability
- Tested end-to-end functionality after updates  
- Verified accuracy and structure of exported files  

### 📦 Project Updates
- Official rebrand to **GitSum**  
- Repository renamed and cleaned up  

---

## [v1.0.0] - 2026-03-25
### ✨ Features
- Generate **commit summaries** from raw commit logs  
- Clean and readable output format  
- Lightweight, browser-based (no setup required)  

### 📦 Included
- Core commit summary generator  
- Basic HTML interface  
- Instant preview of summarized commits  

### 🔮 Planned Improvements
- Export summaries as `.json`, `.md`, `.txt`  
- UI/UX improvements  
- Custom formatting options  

### ⚠️ Notes
- First release; minimal features, intended to improve over time
