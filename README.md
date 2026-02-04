## retro-fan-site-90s-style  
### 90s Anime Fan Site – A Retro Frontend for the Golden Age of Anime

> A lightweight, responsive **frontend-only** website celebrating 90s anime, built with **HTML5** and **CSS3** only (no JavaScript).  
> Designed with a **Windows 95 / Early Web Brutalism** aesthetic.  
> Created by **Francis Remoshan**.

---

### Visuals

<!-- Add your screenshots here after uploading to GitHub (Settings → General → Attachments) -->
<!-- Example:
![Home Page](https://github.com/user-attachments/assets/your-home-screenshot-id)
![History Page](https://github.com/user-attachments/assets/your-history-screenshot-id)
![Gallery Page](https://github.com/user-attachments/assets/your-gallery-screenshot-id)
-->

_Add screenshots of the Home, History, and Gallery pages here once uploaded to your repository._

---

### Features

- **Windows 95 / Early Web Brutalism Aesthetic** – Silver/gray backgrounds (#c0c0c0), navy blue headers (#000080), and high-contrast active states (e.g. neon yellow).
- **3D Beveled UI** – Buttons and panels use `border-style: outset` and `inset` for a classic desktop look.
- **Semantic HTML5** – Uses `<header>`, `<nav>`, `<main>`, `<section>`, and `<footer>`; no div-soup.
- **Responsive Layout** – Max-width 900px, centered; readable on desktops, tablets, and mobile.
- **CSS Flexbox** – Navigation and History page layout built with Flexbox.
- **CSS Grid** – Gallery page uses a 3×3 responsive grid of image cards.
- **Pure CSS Interactivity** – Hover states and “active” page highlighting with no JavaScript.
- **System Fonts** – MS Sans Serif, Tahoma, sans-serif for an authentic retro feel.
- **No Dependencies** – No frameworks or build step; open and run.

---

### Project Structure

```
Retro Fan Site (90s Style)/
├── index.html          # Home – hero marquee, Latest Updates, Visitor Counter
├── history.html        # History – long-form content with image + text sections
├── gallery.html        # Gallery – 3×3 grid of anime image cards
├── style.css           # Shared styles (navigation, layout, responsive)
├── images/             # Image assets (e.g. neon_genesis_evangelion.png, sailor_moon.png)
└── README.md
```

---

### Getting Started

#### Prerequisites

You only need a modern web browser.  
For local development with a simple server (optional), you can use:

- **Node.js** (optional, for running a static server)
- Or a **Live Server** extension in your editor

#### Installation

Clone the repository and open the project:

```bash
# Clone the repository
git clone https://github.com/remoshan/retro-fan-site-90s-style.git

# Move into the project directory
cd retro-fan-site-90s-style
```

Run with a simple static server (optional but recommended):

```bash
# Example using Node's npx (if you have Node installed)
npx serve .

# or using Python 3
python -m http.server 3000

# Then open in your browser:
# http://localhost:3000
```

Or simply open `index.html` directly in your browser (double-click or drag-and-drop into a browser window).

---

### Usage

The site has three pages; the nav is identical on each, with the current page highlighted via the `.active` class.

**Navigation (same on every page):**

```html
<nav>
  <ul>
    <li><a href="index.html" class="active">Home</a></li>
    <li><a href="history.html">History</a></li>
    <li><a href="gallery.html">Gallery</a></li>
  </ul>
</nav>
```

**Active link styling in CSS:**

```css
nav a.active {
  background-color: #ffff00;
  color: #000000;
  border: 2px inset #c0c0c0;
}
```

**Gallery card structure:**

```html
<div class="gallery-card">
  <div class="card-image">
    <img src="images/neon_genesis_evangelion.png" alt="Neon Genesis Evangelion">
  </div>
  <div class="card-caption">Neon Genesis Evangelion</div>
</div>
```

All behavior (hover, active states) is achieved with pure CSS; no JavaScript is required.

---

### Configuration

This is a **static, frontend-only** project. There is no backend, environment variables, or build step.  
To use your own images, place them in the `images/` folder and update the `src` and `alt` attributes in the HTML files accordingly.

---

### Contributing

Contributions are welcome! To propose changes:

1. **Fork** the repository to your GitHub account.
2. **Create a feature branch**:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes** (code, assets, or documentation).
4. **Commit** with a clear message:

   ```bash
   git commit -m "Add: short description of your change"
   ```

5. **Push** your branch:

   ```bash
   git push origin feature/your-feature-name
   ```

6. **Open a Pull Request** against the `main` branch:
   - Describe the motivation, changes, and any relevant screenshots.
   - Reference any related issues if applicable.

Please keep your changes focused and small where possible for easier review.

---

### License

This project is licensed under the **MIT License**.  
The `LICENSE` file is included in the repository root; see it for the full license text and details.