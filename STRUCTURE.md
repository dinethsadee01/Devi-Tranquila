# Devi Tranquil Villa - Project Structure

## 📁 Directory Structure

```
devi-tranquila/
├── index.html                 # Main entry point (for easy access)
├── README.md                 # Project documentation
├── src/                      # Source files
│   ├── pages/               # HTML pages
│   │   ├── index.html       # Home page
│   │   ├── about.html       # About page
│   │   ├── rooms.html       # Rooms page
│   │   ├── gallery.html     # Gallery page
│   │   ├── services.html    # Services page
│   │   ├── contact.html     # Contact page
│   │   ├── blog.html        # Blog page
│   │   ├── faq.html         # FAQ page
│   │   └── 404.html         # Error page
│   └── assets/              # Static assets
│       ├── css/             # Stylesheets
│       │   ├── bootstrap.min.css
│       │   ├── fontawesome.min.css
│       │   ├── animate.css
│       │   ├── slick.min.css
│       │   ├── swiper.min.css
│       │   ├── daterangepicker.css
│       │   ├── lightgallery.min.css
│       │   └── style.css    # Main custom styles
│       ├── js/              # JavaScript files
│       │   ├── jquery-3.6.0.min.js
│       │   ├── bootstrap.min.js
│       │   ├── swiper.min.js
│       │   ├── lightgallery.min.js
│       │   ├── wow.min.js
│       │   ├── moment.min.js
│       │   ├── daterangepicker.min.js
│       │   ├── YTPlayer.min.js
│       │   └── main.js       # Main custom scripts
│       ├── fonts/           # Web fonts
│       │   └── (FontAwesome and other font files)
│       └── images/          # Organized image assets
│           ├── logos/       # Brand logos and favicons
│           │   ├── favicon.ico
│           │   ├── logo.svg
│           │   ├── footer-logo.svg
│           │   ├── 12 2.png (main logo)
│           │   ├── 11 2.png, 11.png, 10 2.png
│           │   └── (other brand assets)
│           ├── icons/       # UI icons and SVG assets
│           │   └── (47 SVG icon files)
│           ├── backgrounds/ # Background and hero images
│           │   ├── home_1.jpg
│           │   ├── home_2.jpg
│           │   ├── home_3.jpg
│           │   └── (background images)
│           ├── avatars/     # Profile and team images
│           │   ├── avatar_*.png
│           │   ├── team_member_*.jpg
│           │   └── author.png
│           ├── gallery/     # Villa and room photos
│           │   ├── IMG_*.JPG (original camera files)
│           │   ├── PHOTO-*.jpg (additional photos)
│           │   └── (UUID-named gallery images)
│           └── common/      # General content images
│               ├── about_us_*.jpg
│               ├── contact_img.jpg
│               ├── signature.png
│               └── (other content images)
└── public/                  # Public assets and utilities
    ├── loading.html         # Loading popup
    ├── video-play.html      # Video player popup
    ├── vimeo-play.html      # Vimeo player popup
    └── youtube-play.html    # YouTube player popup
```

## 🎯 Path References

### From Root (index.html)

- CSS: `src/assets/css/`
- JS: `src/assets/js/`
- Images: `src/assets/images/`

### From Pages (src/pages/\*.html)

- CSS: `../assets/css/`
- JS: `../assets/js/`
- Images: `../assets/images/`

## 📝 File Organization

### Images Categories

- **Logos** (9 files): Brand assets, favicon, SVG logos, PNG logos
- **Icons** (47 files): UI icons, decorative SVGs
- **Backgrounds**: Hero images, page backgrounds
- **Avatars**: Team photos, user avatars
- **Gallery** (375 files): Villa photos, room images (main content)
- **Common** (9 files): General content images, about us photos

### Asset Loading

All assets are properly referenced with the new structure:

- CSS files maintain proper dependency order
- JavaScript files load in correct sequence
- Images are categorized by usage context

## 🔧 Development Notes

- Main entry point remains at root level for easy access
- All source files organized under `src/` directory
- Assets properly categorized for maintainability
- Path references updated throughout all HTML files
- Public utilities separated from main source code

## 🚀 Getting Started

1. Open `index.html` in a web browser
2. All assets will load from the organized structure
3. Navigate between pages using the site navigation
4. No build process required - static HTML/CSS/JS site
