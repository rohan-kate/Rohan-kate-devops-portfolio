# Troubleshooting Guide - Portfolio Not Showing

## Quick Fixes

### 1. Clear Browser Cache
- Press `Ctrl + Shift + Delete` in your browser
- Clear cached images and files
- Refresh the page with `Ctrl + F5`

### 2. Check File Paths
Make sure all files are in the same folder:
- ✅ index.html
- ✅ styles.css
- ✅ script.js

### 3. Open Correctly

**Option A: Direct File Open**
1. Navigate to: `C:\Users\Rohan\OneDrive\Desktop\portfolio`
2. Right-click `index.html`
3. Select "Open with" → Choose your browser (Chrome, Firefox, Edge)

**Option B: Use Python Server (Recommended)**
```powershell
python server.py
```
Then open: http://localhost:8000

**Option C: VS Code Live Server**
1. Install "Live Server" extension in VS Code
2. Right-click `index.html`
3. Select "Open with Live Server"

### 4. Check Browser Console
1. Open the page
2. Press `F12` to open Developer Tools
3. Check the "Console" tab for errors
4. Check the "Network" tab to see if CSS/JS files are loading

### 5. Verify Files Are Not Corrupted
- Check file sizes:
  - index.html should be ~18KB
  - styles.css should be ~15KB
  - script.js should be ~6KB

### 6. OneDrive Sync Issues
If files are in OneDrive, make sure they're fully synced:
- Check OneDrive icon in system tray
- Wait for sync to complete
- Try opening from local path instead

### 7. Test with Simple HTML
Open `test.html` first to verify your browser works, then try `index.html`

## Common Issues

**Blank Page:**
- Check browser console (F12) for errors
- Verify CSS file is loading (Network tab)
- Try a different browser

**Styles Not Loading:**
- Check if `styles.css` exists in same folder
- Verify file path in HTML: `<link rel="stylesheet" href="styles.css">`
- Check browser console for 404 errors

**JavaScript Not Working:**
- Check if `script.js` exists in same folder
- Verify file path: `<script src="script.js"></script>`
- Check browser console for errors

## Still Not Working?

1. Try opening in Incognito/Private mode
2. Disable browser extensions temporarily
3. Try a different browser
4. Check Windows Firewall isn't blocking local files
5. Verify you have read permissions on the files
