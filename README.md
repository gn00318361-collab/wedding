# Wedding Opening Slideshow

A beautiful, single-file HTML wedding opening slideshow with auto-play animations, particle effects, and responsive design. Perfect for projecting at wedding banquets to welcome guests before the ceremony begins.

## Demo

> Replace with your GitHub Pages URL after deployment:
>
> `https://<your-username>.github.io/wedding-opening/`

## Features

- 22 slides with smooth fade transitions and auto-play timing
- Falling leaf particle animation (canvas-based)
- Responsive layout for projectors, laptops, and tablets
- Keyboard and click navigation (Arrow keys / Space / Click)
- Progress bar and slide counter
- Loading heart animation
- Google Fonts: Noto Serif TC, Great Vibes, Playfair Display
- Zero dependencies, single HTML file, no build step required

## Slide Flow

| # | Content | Duration |
|---|---------|----------|
| 1 | Welcome + couple photos | 7s |
| 2 | Loading heart animation | 5s |
| 3 | "We are getting married!" | 6s |
| 4 | Who we are (childhood photos) | 9s |
| 5 | Transition: "Then..." | 3s |
| 6 | "We fell in love!" (animated) | 8s |
| 7 | "Wedding is about to start" | 6s |
| 8 | "Please take your seats" | 6s |
| 9 | "Phones on silent" | 6s |
| 10 | "A great day to gather" | 6s |
| 11 | "Thank you for coming" | 5s |
| 12 | Reminders intro | 6s |
| 13 | "Enjoy the food" | 6s |
| 14 | "Drinks are unlimited" | 6s |
| 15 | "We have a photographer" | 5s |
| 16 | "Don't block the camera" | 6s |
| 17 | "Tag us on Instagram" | 7s |
| 18 | Transition: "Lastly" | 3s |
| 19 | "It's our first time getting married" | 7s |
| 20 | "But we're ready!" | 5s |
| 21 | "Give us your cheers!" | 7s |
| 22 | "Our wedding begins now" | 8s |

## Quick Start

1. Clone or download this repository.
2. Put your photos in the same folder as `wedding-opening.html`.
3. Open `wedding-opening.html` in a browser.
4. The slideshow will auto-play immediately.

## How to Customize

### Replace Photos

All images are referenced by filename in the HTML. Replace the following files with your own photos (keep the same filenames, or update the `src` attributes in the HTML):

| Filename | Description |
|----------|-------------|
| `男生獨照.jpg` | Groom solo photo (slide 1) |
| `女生獨照.jpg` | Bride solo photo (slide 1) |
| `3.we are getting married！.jpg` | Couple photo (slide 3) |
| `4.我們是(小宣廷1).jpg` ~ `(小宣廷3).jpg` | Groom childhood photos (slide 4) |
| `4.我們是(小依潔1).jpg` ~ `(小依潔3).jpg` | Bride childhood photos (slide 4) |
| `6.我們相愛啦！(...).jpg` | Bride photo for love slide (slide 6) |
| `1.擷取宣廷.jpg` | Groom photo for love slide (slide 6) |
| `7.婚禮即將開始囉～.jpg` | Couple photo (slide 7) |
| `8.請大家盡快就座.jpg` | Couple photo (slide 8) |
| `10. 今天是適合相聚的好日子！.jpg` | Couple photo (slide 10) |
| `16. 也請不要擋到攝影師的鏡頭唷.jpg` | Fun photo (slide 16) |
| `19.因為我們是第一次結婚.jpg` | Couple photo (slide 19) |
| `22. 我們的婚禮要開始囉.jpg` | Couple photo (slide 22) |

### Edit Names and Text

Open `wedding-opening.html` in any text editor and search/replace:

- `Tim` / `Eva` — couple's English names
- `宣廷` / `依潔` — couple's Chinese names
- `1994年出生` — birth years
- `eva93510` / `5xuan_tingwu` — Instagram handles
- Any slide text can be freely edited

### Adjust Timing

Find the `durations` array in the `<script>` section to change how long each slide displays (values in milliseconds):

```javascript
const durations = [
  7000,  // 1: Welcome
  5000,  // 2: Loading
  // ... edit as needed
];
```

### Color Scheme

CSS custom properties at the top of the file control the color palette:

```css
:root {
  --forest: #2C5F2D;    /* Primary green */
  --sage: #84B59F;       /* Light green */
  --cream: #FDF8F0;      /* Background cream */
  --warm: #D4A574;       /* Warm accent */
  --gold: #C4A265;       /* Gold accent */
  --pink: #E8B4B8;       /* Pink accent */
}
```

## Deploy to GitHub Pages

1. Create a new repository on GitHub.
2. Upload `wedding-opening.html` (rename to `index.html`) and all image files.
3. Go to **Settings > Pages**, set source to `main` branch.
4. Your slideshow will be live at `https://<username>.github.io/<repo-name>/`.

## Navigation

| Input | Action |
|-------|--------|
| Auto | Slides advance automatically |
| → / Space / Enter / Click | Next slide |
| ← | Previous slide |

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). Requires an internet connection for Google Fonts loading; falls back to system serif fonts if offline.

## License

MIT License — free to use, modify, and share.
