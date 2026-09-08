# Navbar — Sliding Sidebar Menu (CSS Project)

A pure HTML & CSS mini-project featuring a full-screen background image with a toggleable, sliding sidebar navigation menu. The menu opens and closes using a checkbox-driven CSS trick — no JavaScript required.

## Features

- **Full-screen hero background** using a background image (`minipro.jpg`)
- **Slide-in sidebar menu** toggled by a hamburger icon, built entirely with the CSS `:checked` sibling selector (no JS)
- **Animated open/close icons** — hamburger icon fades out and a close (✕) icon fades in when the menu is open
- **Menu items with icons** (Gallery, Shortcuts, Exhibits, Events, Store, Contact, Feedback, Logout) using Font Awesome icons
- **Social media links** (Facebook, Twitter, Instagram, YouTube, LinkedIn) fixed near the bottom of the sidebar
- **Smooth CSS transitions** on hover and toggle for a polished feel
- **Google Fonts** (Poppins, Roboto, Special Gothic) for typography

## Tech Stack

- **HTML5**
- **CSS3** (Flexbox-free, position/transition-based layout)
- **Font Awesome 6.4.0** (via CDN) for icons
- **Google Fonts** (via CDN) for typography

## Project Structure

```
Navbar/
├── minipro.html    # Markup — hero section, sidebar, menu items, social links
├── stylemp.css     # Styling — layout, sidebar animation, hover effects
└── minipro.jpg     # Background image used by the hero section
```

## How the Sidebar Toggle Works

The menu uses a hidden checkbox (`#check`) paired with CSS sibling selectors — a common no-JavaScript technique:

- A `<label for="check">` wraps the hamburger icon; clicking it toggles the checkbox.
- `#check:checked ~ .sidebar_menu` slides the sidebar into view (`left: -300px` → `left: 0`).
- `#check:checked ~ .btn_one i` fades out the hamburger icon.
- `#check:checked ~ .sidebar_menu .btn_two i` fades in the close (✕) icon inside the sidebar.

## Getting Started

No build tools or dependencies to install — it's a static HTML/CSS page.

1. **Clone the repository**

   ```bash
   git clone https://github.com/sunil502/Basic-Project.git
   cd Basic-Project/Navbar
   ```

2. **Open it in a browser**

   Simply open `minipro.html` directly in your browser, or serve it locally:

   ```bash
   npx serve .
   ```

   or, with Python:

   ```bash
   python3 -m http.server
   ```

   Then visit `http://localhost:8000/minipro.html`.

## Usage

- Click the hamburger icon (☰) in the top-left corner to open the sidebar.
- Click the close icon (✕) inside the open sidebar to hide it again.
- Hover over menu items and social icons to see the interactive hover effects.

## Notes

- All navigation links (`href="#"`) are placeholders — wire them up to real pages/routes as needed.
- The `minipro.jpg` file must remain in the same folder as `stylemp.css` since it's referenced as a relative background image.

## License

No license has been specified for this project yet. Consider adding one (e.g., MIT) if you plan to share or accept contributions.
