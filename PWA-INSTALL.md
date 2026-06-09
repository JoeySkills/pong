# Installing PONG as an iPhone App (PWA)

Your Pong game is now a Progressive Web App! Here's how to install it on your iPhone:

## Option 1: Install from Local Server (Testing)

1. **Get your computer's IP address:**
   ```bash
   ipconfig getifaddr en0  # WiFi
   # or
   ipconfig getifaddr en1  # Ethernet
   ```

2. **Start the server:**
   ```bash
   cd /Users/jscalia/ClaudeProjects/pong
   python3 -m http.server 8080
   ```

3. **On your iPhone** (must be on same WiFi):
   - Open Safari
   - Go to `http://YOUR-IP-ADDRESS:8080/pong.html`
   - Tap the Share button (square with arrow)
   - Scroll down and tap "Add to Home Screen"
   - Tap "Add"

4. **Done!** You'll see the PONG icon on your home screen. Tap it to play fullscreen.

## Option 2: Deploy Online (Permanent)

To make it permanently accessible, deploy to a free hosting service:

### GitHub Pages (Recommended)
1. Create a GitHub repository
2. Push these files: `pong.html`, `manifest.json`, `service-worker.js`, `icon-192.png`, `icon-512.png`
3. Enable GitHub Pages in repo settings
4. Visit `https://YOUR-USERNAME.github.io/REPO-NAME/pong.html`
5. Add to home screen from Safari

### Other Options
- **Netlify**: Drag & drop the folder at netlify.com/drop
- **Vercel**: `vercel --prod` (install with `npm i -g vercel`)
- **Cloudflare Pages**: Free hosting with custom domain support

## Features
- ✓ Works offline after first load
- ✓ Fullscreen experience
- ✓ Touch controls optimized for mobile
- ✓ Launches like a native app
- ✓ No App Store required

## Files Created
- `manifest.json` - App metadata and icons
- `service-worker.js` - Offline caching
- `icon-192.png` & `icon-512.png` - App icons
- `pong.html` - Updated with PWA support

## Troubleshooting
- **"Add to Home Screen" not showing?** Make sure you're using Safari (not Chrome)
- **Icons not loading?** Clear Safari cache and reload
- **Service worker errors?** Must be served over HTTP/HTTPS (not file://)
