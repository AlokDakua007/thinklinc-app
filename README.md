# THINK LINC — Mobile App (HTML/CSS)

A clickable HTML/CSS build of the Figma **Mobile APP UI** page (three Android Compact screens, 412 × 917).

## Flow

1. **`index.html` – Splash.** Shows the THINK LINC logo, then moves to login after about 2 seconds. You can also tap to skip.
2. **`login.html` – Login.** Pick a role (Dealer, Retailer or Other) and type *anything* into both fields. Press **Login**. If a field is empty, the form shakes and stays on the page.
3. **`home.html` – Home.** Shows the greeting (which follows the time of day), point balance, banner, quick actions, the Redeem section and the bottom tab bar.
   - The menu icon goes back to login.

## Run it

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .        # or: python3 -m http.server
```

How it displays:

- **Desktop:** the app shows as a 412 × 917 phone, matching the Figma frames.
- **Phone:** it fills the screen and hides the design's mock status bar.

## Structure

```
index.html   splash screen
login.html   login screen
home.html    home dashboard
styles.css   all styles (tokens in :root)
assets/      logo, banner, redeem art and icons exported from Figma (webp/svg)
fonts/       Inter (fallback for SF Pro)
```

## Fonts

The design uses **SF Pro**. It is used if it is installed locally. Otherwise the page falls back to Inter, size-matched. SF Pro is not bundled because of its licence.
