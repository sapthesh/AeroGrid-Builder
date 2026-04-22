# AeroGrid Builder
<a href="https://hits.sh/github.com/sapthesh/AeroGrid-Builder/"><img alt="Hits" src="https://hits.sh/github.com/sapthesh/AeroGrid-Builder.svg?view=today-total&color=fe7d37"/></a> 

  <strong>A revolutionary, high-performance WordPress visual page builder</strong><br>
  


---

## Why AeroGrid?

**Most WordPress page builders add 500KB+ of JavaScript and CSS to every page.** AeroGrid is fundamentally different—built from the ground up for performance and simplicity.

### Zero-Bloat Architecture
- Uses **native CSS Grid** instead of nested div tables
- No heavy frameworks or dependencies
- 100% theme agnostic—inherits your active theme's styles
- Only loads assets for what's actually used (conditional loading)

### 100x Smaller, 100x Faster
- **25.84 kB gzipped** bundle (vs Other's 500KB+)
- Native browser APIs instead of custom rendering engines
- Zero runtime CSS generation
- No page weight penalty on the frontend

### Built for Modern WordPress
- Works with any WordPress 6.0+ theme
- No forced templates or design restrictions
- Pure HTML output—no inline styles or wrapper divs

---

## Revolutionary Features

### Universal Layout Parser
Import existing pages from **Elementor** or **WPBakery** and instantly convert them to clean, semantic markup. Export your AeroGrid layouts as portable JSON for backup or migration.

### Built-in Performance Profiler
See exactly how your page performs before publishing:
- DOM node count
- Nesting depth analysis
- Estimated render size
- Load time predictions

### A11y Enforcer
Built-in accessibility compliance checks:
- Auto-detection of missing alt text on images
- Contrast ratio validation for text colors
- Keyboard navigation path analysis
- Real-time accessibility score

### Revision History
Full undo/redo support with **20-state history**:
- Press `Ctrl+Z` / `Cmd+Z` to undo
- Press `Ctrl+Y` / `Cmd+Y` to redo
- Visual timeline of all changes

### Floating Contextual Toolbar
No more sidebar clutter—edit directly where you work:
- Toolbar floats near your current selection
- Context-aware actions based on selected element
- Minimal, distraction-free interface

### Inline Text Editing
Edit content exactly as it appears:
- `contenteditable` for headings and paragraphs
- Real-time WYSIWYG experience
- No separate content panels to manage

---

## Installation

1. **Upload** the `aerogrid-builder` folder to `/wp-content/plugins/`
2. **Activate** the plugin via WordPress Plugins menu
3. **Edit** any post or page by clicking "Edit with AeroGrid"
4. **Drag** modules from the sidebar onto your canvas
5. **Export/Import** templates via the Template Library

---

## Technical Details

| Requirement | Details |
|-------------|---------|
| **PHP Version** | 8.0+ |
| **WordPress** | 6.0+ |
| **Frontend Framework** | Preact (3x smaller than React) |
| **Build Tool** | Vite |
| **Grid System** | Native CSS Grid (no custom framework) |
| **JS Bundle** | 25.84 kB gzipped |
| **CSS Bundle** | ~5 kB (grid engine only) |

---

## Development

### Prerequisites
- Node.js 18+
- npm or bun

### Setup

```bash
# Install dependencies
npm install

# Start development server (watch mode)
npm run dev

# Build production assets
npm run build
```

### Project Structure

```
aerogrid-builder/
├── aerogrid-builder.php     # Main plugin file
├── includes/                # PHP classes
│   ├── class-aerogrid-db.php
│   ├── class-aerogrid-admin.php
│   └── class-aerogrid-admin-page.php
├── src/                     # Source files
│   ├── editor/              # Editor UI components
│   ├── renderer/            # Layout rendering logic
│   ├── profiler/            # Performance profiling
│   └── modules/             # Built-in modules
├── assets/                  # Built assets (production)
│   ├── js/
│   │   └── editor.js
│   └── css/
│       ├── editor.css
│       └── grid-engine.css
└── README.md
```

---

## License

This project is licensed under the GNU General Public License v2 or later.

---

## Credits

**AeroGrid Builder** - Built with performance, simplicity, and accessibility in mind.
