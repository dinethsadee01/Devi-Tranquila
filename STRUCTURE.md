# Devi Tranquil Villa - Project Structure

## 📁 Current Project Structure

```
devi-tranquila/
├── index.html                    # Main homepage
├── src/
│   ├── pages/                    # All sub-pages
│   │   ├── about.html
│   │   ├── contact.html
│   │   ├── gallery.html
│   │   ├── rooms.html
│   │   ├── services.html
│   │   ├── blog.html
│   │   ├── faq.html
│   │   ├── 404.html
│   │   └── index.html
│   └── assets/                   # Static assets
│       ├── css/
│       │   ├── global-styles.css  # Centralized global styles
│       │   ├── bootstrap.min.css
│       │   ├── fontawesome.min.css
│       │   ├── animate.css
│       │   ├── slick.min.css
│       │   ├── swiper.min.css
│       │   ├── daterangepicker.css
│       │   ├── lightgallery.min.css
│       │   └── style.css
│       ├── js/
│       │   ├── jquery-3.6.0.min.js
│       │   ├── wow.min.js
│       │   ├── jquery.slick.min.js
│       │   ├── swiper.min.js
│       │   ├── moment.min.js
│       │   ├── daterangepicker.min.js
│       │   ├── lightgallery.min.js
│       │   ├── YTPlayer.min.js
│       │   └── main.js
│       ├── images/
│       │   ├── logos/
│       │   │   ├── logo.svg
│       │   │   ├── favicon.ico
│       │   │   └── [other logo files]
│       │   ├── backgrounds/
│       │   │   ├── home_1.jpg
│       │   │   ├── home_2.jpg
│       │   │   └── [other background files]
│       │   ├── gallery/
│       │   │   ├── IMG_0515.JPG
│       │   │   ├── IMG_0516.JPG
│       │   │   └── [other gallery files]
│       │   ├── avatars/
│       │   │   ├── avatar_1.png
│       │   │   ├── team_member_1.jpg
│       │   │   └── [other avatar files]
│       │   ├── common/
│       │   │   ├── about_us_1.jpg
│       │   │   ├── contact_img.jpg
│       │   │   └── [other common files]
│       │   ├── icons/
│       │   │   ├── loading.svg      # LightGallery loading spinner
│       │   │   ├── video-play.svg   # HTML5 video play button
│       │   │   ├── youtube-play.svg # YouTube video play button
│       │   │   ├── vimeo-play.svg  # Vimeo video play button
│       │   │   ├── bbq.svg
│       │   │   ├── coffee.svg
│       │   │   └── [other icon files]
│       │   └── [other image folders]
│       └── fonts/
│           ├── fa-brands-400.ttf
│           ├── fa-regular-400.ttf
│           ├── fa-solid-900.ttf
│           └── [other font files]
├── README.md                     # Project documentation
└── STRUCTURE.md                  # This file
```

## 🎯 Folder Purposes

### ✅ **Root Directory**
- `index.html` - Main homepage of the website
- Contains the primary landing page with hero section, rooms preview, etc.

### ✅ **src/pages/**
- Contains all sub-pages of the website
- Each page is a complete HTML file with proper navigation
- Pages include: About, Contact, Gallery, Rooms, Services, Blog, FAQ, 404

### ✅ **src/assets/**
- **css/** - All stylesheets including the centralized global styles
- **js/** - All JavaScript files for functionality
- **images/** - All images organized by category
- **fonts/** - Font files for the website

## 🔧 File Organization Best Practices

### ✅ **HTML Files**
- Main page (`index.html`) stays in root for easy access
- Sub-pages go in `src/pages/` for organization
- Each page is self-contained with proper navigation

### ✅ **CSS Files**
- `global-styles.css` - Centralized global styles (no duplication)
- Other CSS files - Framework and library stylesheets
- All CSS files in `src/assets/css/`

### ✅ **JavaScript Files**
- All JS files in `src/assets/js/`
- Includes jQuery, plugins, and custom scripts
- `main.js` contains custom functionality

### ✅ **Images**
- Organized by category in `src/assets/images/`
- Logos, backgrounds, gallery, icons, etc.
- Proper naming conventions for easy management

### ✅ **LightGallery Integration**
- **Fixed CSS paths** - Updated `lightgallery.min.css` to use proper SVG icons
- **Created SVG icons** - Loading spinner and video play buttons
- **Proper functionality** - LightGallery works correctly with video players

## 🚀 Recent Improvements

### ✅ **Removed Public Folder**
- Eliminated unnecessary placeholder files
- Cleaned up project structure
- No impact on functionality

### ✅ **Fixed LightGallery Paths**
- **Before**: CSS referenced HTML files as background images
- **After**: CSS references proper SVG icons
- **Result**: LightGallery video players work correctly

### ✅ **Created Missing Icons**
- `loading.svg` - Animated loading spinner for LightGallery
- `video-play.svg` - HTML5 video play button
- `youtube-play.svg` - YouTube video play button
- `vimeo-play.svg` - Vimeo video play button

## 📋 File Naming Conventions

### ✅ **HTML Files**
- Use lowercase with hyphens: `about.html`, `contact.html`
- Descriptive names that indicate content
- Consistent naming across all pages

### ✅ **CSS Files**
- `global-styles.css` - Centralized styles
- Framework files keep original names
- Use descriptive names for custom CSS

### ✅ **JavaScript Files**
- Framework files keep original names
- `main.js` - Custom functionality
- Use descriptive names for custom scripts

### ✅ **Image Files**
- Use descriptive names
- Include dimensions if relevant
- Organize by category in subfolders

### ✅ **SVG Icons**
- Use descriptive names: `loading.svg`, `video-play.svg`
- Consistent naming for related icons
- Proper organization in `icons/` folder

## 🎯 Benefits of This Structure

### ✅ **Organization**
- Clear separation of concerns
- Easy to find and manage files
- Logical grouping of assets

### ✅ **Maintainability**
- Centralized CSS prevents duplication
- Easy to update global styles
- Clear file locations

### ✅ **Scalability**
- Easy to add new pages
- Simple to add new assets
- Clear structure for growth

### ✅ **Performance**
- Optimized file organization
- Proper asset caching
- Efficient loading structure

### ✅ **Functionality**
- All features work correctly
- LightGallery video players functional
- Proper loading states and play buttons

## 🔧 Path References

### ✅ **From Root (index.html)**
```html
<link rel="stylesheet" href="src/assets/css/global-styles.css">
<script src="src/assets/js/main.js"></script>
<img src="src/assets/images/logos/logo.png">
```

### ✅ **From Sub-pages (src/pages/*.html)**
```html
<link rel="stylesheet" href="../assets/css/global-styles.css">
<script src="../assets/js/main.js"></script>
<img src="../assets/images/logos/logo.png">
```

### ✅ **LightGallery CSS Paths**
```css
/* Loading spinner */
background: url(../images/icons/loading.svg) center center no-repeat;

/* Video play buttons */
background: url(../images/icons/video-play.svg) no-repeat;
background: url(../images/icons/youtube-play.svg) no-repeat;
background: url(../images/icons/vimeo-play.svg) no-repeat;
```

## 🚀 Future Development

### ✅ **Adding New Pages**
1. Create new HTML file in `src/pages/`
2. Include proper navigation links
3. Reference assets with correct relative paths

### ✅ **Adding New Styles**
1. Update `src/assets/css/global-styles.css`
2. Keep styles centralized and organized
3. Use consistent naming conventions

### ✅ **Adding New Images**
1. Place in appropriate `src/assets/images/` subfolder
2. Use descriptive file names
3. Optimize for web use

### ✅ **Adding New Scripts**
1. Place in `src/assets/js/`
2. Update HTML files to include new scripts
3. Follow existing naming conventions

---

**This structure provides a clean, organized, and maintainable foundation for your Devi Tranquil Villa website with all functionality working correctly!**
