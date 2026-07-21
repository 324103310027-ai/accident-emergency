# Accident Emergency Alert System - Static Web Version

This is the fully static, client-side version of the **Accident Emergency Alert System**, designed specifically for hosting on **GitHub Pages** (`https://324103310027-ai.github.io/accident-emergency-system/`).

## Features & Implementation
- **Local Storage Emulation**: Registration, login, emergency contacts, and incident logs are handled entirely in the browser using `localStorage`.
- **Pre-configured Admin Account**: You can sign in using:
  - **Email**: `admin@emergency.com`
  - **Password**: `admin123`
- **Live Mapping & Reverse Geocoding**: HTML5 Geolocation API maps your current position. Integrated Nominatim reverse-geocoder resolves physical addresses dynamically.
- **Nearest Services Locator**: Connects to the keyless OpenStreetMap Overpass engine to query, map, and list the nearest 5 Hospitals and Police Stations in real-time.
- **Pulsing SOS Button**: Designed with a 1.5s hold requirement (with pulsing visual cues) to prevent accidental triggers.

---

## Deployment to GitHub Pages

To deploy this code to your repository:

### Option A: Upload via GitHub Web Interface
1. Go to your repository on GitHub: `https://github.com/324103310027-ai/accident-emergency-system`
2. Click **Add file** -> **Upload files**.
3. Drag and drop all the files from this folder:
   - `index.html`
   - `login.html`
   - `register.html`
   - `dashboard.html`
   - `contacts.html`
   - `admin.html`
   - `alert_detail.html`
   - `css/` (including `style.css`)
   - `js/` (including `main.js`)
4. Click **Commit changes**.
5. Go to **Settings** -> **Pages** in your repository.
6. Under **Build and deployment**, set the source to **Deploy from a branch** and select the **main** branch (with root `/` folder), then click **Save**.
7. Wait a couple of minutes, and your site will be live at `https://324103310027-ai.github.io/accident-emergency-system/`!

---

### Option B: Push via Git Terminal
If you have Git installed, open your terminal/command prompt and run:
```bash
git init
git add .
git commit -m "Initial commit of static page code"
git branch -M main
git remote add origin https://github.com/324103310027-ai/accident-emergency-system.git
git push -u origin main --force
```
*(Make sure to verify settings in GitHub -> Settings -> Pages as described in Step 5/6 above)*
