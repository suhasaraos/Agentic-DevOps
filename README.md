# Presentation Template

A clean, modern presentation template with keyboard/touch navigation and mobile-responsive design.

## Quick Start

1. **Edit `config.js`** - Set your presentation title, presenter info, and total slides
2. **Edit `slide1.html`** - Customize your first slide content
3. **Open `index.html`** in a browser to start

## What's Included

```
template/
├── index.html              # Welcome/landing page
├── slide1.html            # First slide (example)
├── slide-template.html    # Template for creating new slides
├── config.js              # Presentation configuration
├── navbar.js              # Navigation bar component
├── navigation.js          # Slide navigation logic
├── styles.css             # All styling
├── images/                # Place your images here
└── README.md             # This file
```

## Configuration

Edit `config.js` to customize:

```javascript
const presentationConfig = {
    presenter: {
        name: "Your Name",
        title: "Your Title",
        company: "Your Company"
    },
    event: {
        name: "Your Presentation Title",
        date: "Month Year",
        totalSlides: 1  // Update when you add slides
    },
    hiddenSlides: []  // Hide specific slides: [2, 5]
};
```

## Creating New Slides

1. Copy `slide-template.html` → `slide2.html` (or slideX.html)
2. Replace placeholder content in the slide-content section
3. Update `[SLIDE_NUMBER]` and `[TOTAL_SLIDES]` in the slide indicator
4. Update `totalSlides` in `config.js`

### Example Content Components

**Simple Title:**
```html
<h1>Your Title</h1>
<h3 class="subtitle">Your Subtitle</h3>
```

**Icon with Title:**
```html
<i class="bi bi-rocket-takeoff github-icon" style="color: var(--accent);"></i>
<h2>Your Title</h2>
```

**Content with List:**
```html
<div class="content-section">
    <p class="intro-text">Introduction text</p>
    <div class="content-list">
        <ul>
            <li>Point 1</li>
            <li>Point 2</li>
            <li>Point 3</li>
        </ul>
    </div>
</div>
```

**Cards (2-3 columns):**
```html
<div class="theme-cards">
    <div class="theme-card">
        <i class="bi bi-cpu"></i>
        <h3>Title</h3>
        <p>Description</p>
    </div>
    <div class="theme-card">
        <i class="bi bi-shield-check"></i>
        <h3>Title</h3>
        <p>Description</p>
    </div>
</div>
```

## Navigation

- **Desktop:** 
  - Arrow keys (← →)
  - Spacebar (next)
  - Click left/right 50% of screen
- **Mobile:** 
  - Swipe left/right
  - Tap left/right 25% of screen

## Features

✅ Fully responsive (mobile, tablet, desktop)  
✅ Keyboard & touch navigation  
✅ PowerPoint-like click navigation  
✅ Hide specific slides  
✅ Config-driven content  
✅ Bootstrap 5 & Icons included  
✅ Dark theme optimized  

## Bootstrap Icons

Browse icons at: https://icons.getbootstrap.com/

Common icons:
- `bi-rocket-takeoff` - Launch
- `bi-cpu` - Technology
- `bi-shield-check` - Security
- `bi-building` - Enterprise
- `bi-graph-up` - Growth
- `bi-code-slash` - Code
- `bi-lightning` - Fast
- `bi-people` - Team

## Tips

- Keep slide content concise and visual
- Use high-contrast colors for readability
- Test on mobile devices
- Place images in the `images/` folder
- Update `totalSlides` in config when adding slides
- Use hidden slides for optional content

## Customization

All colors and styles are in `styles.css` with CSS variables:

```css
:root {
    --bg-primary: #0d1117;
    --bg-secondary: #161b22;
    --text-primary: #c9d1d9;
    --text-secondary: #8b949e;
    --accent: #39d98a;
    --accent-hover: #2ea472;
    --border-color: #30363d;
}
```

## Browser Support

Modern browsers recommended:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)

---

**Ready to present!** Just edit `config.js` and start customizing your slides.
