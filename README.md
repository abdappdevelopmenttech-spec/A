# ABD App Development Tech

A modern, responsive company website for **ABD App Development Tech**, a mobile app development business based in Nigeria with 100+ Android apps published on Google Play.

The whole site lives in a single HTML file with no build step and no dependencies to install.

## Features

- **Single-page navigation** with four views: Home, Our Apps, About Us, and Contact
- **Dynamic app catalog** rendered from a JavaScript data array, with category filters (Country Radio FM, Utilities & Tools, Audio & Voice)
- **Responsive design** for desktop, tablet, and mobile, including a slide-in mobile menu
- **Dark theme** with gradient accents, a phone mockup hero, and hover animations
- **Leadership section** presenting the CEO and directors
- **Contact page** with business email, location, and a message form

## Tech Stack

- HTML5, CSS3 (custom properties, Grid, Flexbox), and vanilla JavaScript
- [Inter](https://fonts.google.com/specimen/Inter) font via Google Fonts
- [Font Awesome 6.4](https://fontawesome.com/) icons via cdnjs

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```
2. Open `abd-app-development-tech.html` in your browser.

An internet connection is needed to load the fonts and icons from their CDNs.

## Project Structure

```
.
├── abd-app-development-tech.html   # Full website (HTML, CSS, JS)
└── README.md
```

## Customization

### Add or edit apps

Edit the `appData` array in the `<script>` section at the bottom of the HTML file:

```js
{
  id: 9,
  title: "Your App Name",
  category: "radio",              // radio | utility | audio
  categoryName: "Country Radio FM",
  icon: "fa-radio",               // any Font Awesome icon class
  bg: "linear-gradient(135deg, #059669 0%, #10b981 100%)",
  description: "Short description of the app.",
  featured: false                 // true = shown on the Home page
}
```

To link a card to a real Google Play listing, replace the `https://play.google.com` URL inside `createAppCardHTML()` with a per-app link.

### Change colors

Update the CSS variables in the `:root` block at the top of the `<style>` section (for example `--primary`, `--accent`, `--bg-dark`).

### Contact form

The form currently shows a confirmation message only and does not send data anywhere. To receive messages, connect it to a form service such as Formspree or Netlify Forms, or to your own backend.

## Deploy to GitHub Pages

1. Rename `abd-app-development-tech.html` to `index.html`.
2. Push the repository to GitHub.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
5. Your site will be live at `https://<your-username>.github.io/<your-repo>/`.

## Contact

- **Email:** [abdappdevelopment.tech@gmail.com](mailto:abdappdevelopment.tech@gmail.com)
- **Location:** Nigeria, Africa

## License

&copy; 2026 ABD App Development Tech. All rights reserved.
