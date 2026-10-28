# Al-Husseiny Contracting (الحسيني للمقاولات)

## 1. Project Overview

**الحسيني للمقاولات** (Al-Husseiny Contracting) is an Arabic right-to-left (RTL) static website for a construction and general contracting company based in Aswan, Egypt. The website showcases the company's background, portfolio of residential and commercial projects, contracting and finishing services, customer contact options, and educational articles on construction and finishing techniques.

## 2. Features

- **Homepage:** Features a video hero section, company introduction, service highlights, featured projects, latest articles, and customer contact options.
- **About Us Page (`about-us/`):** Detailed overview of company experience, mission, vision, statistics, and work philosophy.
- **Projects Gallery (`projects/`):** Categorized portfolio with project cards, interactive project modal with image gallery slider, details, and direct contact actions.
- **Articles & Blog (`articles/`):** Articles index with pagination and dedicated article pages covering:
  - Building Bricks Selection (`articles/bricks/`)
  - Choosing the Right Contractor (`articles/choosing-contractor/`)
  - Concrete Works and Specifications (`articles/concrete/`)
  - Electrical Works and Installations (`articles/electricity/`)
  - Interior & Exterior Finishing Levels (`articles/finishing/`)
  - Plumbing Essentials and Installations (`articles/plumbing/`)
- **Direct WhatsApp Inquiry:** Interactive quote and inquiry modal that formats submitted project details directly into WhatsApp messages.
- **Interactive UI:** Smooth scroll powered by Lenis, responsive navigation with mobile drawer menu, scroll-to-top button, and on-scroll reveal animations.
- **Custom 404 Page (`404.html`):** Clean error page with direct navigation back to the homepage.
- **SEO & Discovery:** Meta tags, Open Graph and Twitter cards, structured JSON-LD schemas (`LocalBusiness`, `Organization`, `Article`, `CollectionPage`, `BreadcrumbList`), `robots.txt`, and `sitemap.xml`.

## 3. Technologies Used

- **HTML5:** Semantic markup structured for right-to-left (RTL) Arabic content.
- **CSS3:** Custom stylesheet (`css/style.css`), reset styling (`css/normalize.css`), and local Font Awesome styles (`css/all.min.css`).
- **Vanilla JavaScript:** Client-side functionality in `js/script.js` (DOM interactions, dynamic card rendering, modal dialogs, WhatsApp link generation, image slider).
- **Tailwind CSS (CDN):** Utility-first styling framework configured inline with custom color theme and Tajawal typography.
- **Lenis (CDN):** Smooth scrolling library.
- **Font Awesome (CDN & Local):** Iconography via CDN with local fallback in `css/all.min.css` and `webfonts/`.
- **Google Fonts (CDN):** Tajawal Arabic typeface.

The project is entirely static and requires no package manager, compiler, bundler, or runtime dependencies.

## 4. Project Structure

```text
Al-Husseiny/
├── about-us/
│   └── index.html                  # About Us page
├── article-images/                 # Cover and featured images for blog articles
│   ├── brick.png
│   ├── conc.png
│   ├── elic.png
│   ├── fin.png
│   └── Plum.png
├── articles/                       # Articles section
│   ├── bricks/
│   │   └── index.html              # Article: Building Bricks Guide
│   ├── choosing-contractor/
│   │   └── index.html              # Article: Choosing a Contractor Guide
│   ├── concrete/
│   │   └── index.html              # Article: Concrete Works Guide
│   ├── electricity/
│   │   └── index.html              # Article: Electrical Finishing Guide
│   ├── finishing/
│   │   └── index.html              # Article: Finishing Types Guide
│   ├── plumbing/
│   │   └── index.html              # Article: Plumbing Installations Guide
│   └── index.html                  # Articles archive / blog listing
├── css/                            # Stylesheets
│   ├── all.min.css                 # Local Font Awesome stylesheet
│   ├── normalize.css               # CSS reset
│   └── style.css                   # Custom global site styles
├── images/                         # Brand assets, site icons, and page media
│   ├── 2.png                       # Projects section hero background
│   ├── 3.png                       # Articles section hero background
│   ├── brick-wall.png              # Pattern asset
│   ├── Hero.mp4                    # Homepage hero video
│   ├── hero-video.mp4              # About Us page hero video
│   ├── icon.png                    # Site favicon / icon
│   ├── logo.png                    # Brand logo
│   └── profile.png                 # Profile and featured imagery
├── js/                             # Client-side scripts
│   └── script.js                   # Main application script
├── projects/
│   └── index.html                  # Projects portfolio page
├── webfonts/                       # Font Awesome webfont binary files
│   ├── fa-brands-400.ttf
│   ├── fa-brands-400.woff2
│   ├── fa-regular-400.ttf
│   ├── fa-regular-400.woff2
│   ├── fa-solid-900.ttf
│   ├── fa-solid-900.woff2
│   ├── fa-v4compatibility.ttf
│   └── fa-v4compatibility.woff2
├── 404.html                        # Custom 404 error page
├── google58051ffbc8570adc.html     # Google Search Console site verification file
├── index.html                      # Homepage
├── README.md                       # Project documentation
├── robots.txt                      # Search engine crawler directives
└── sitemap.xml                     # XML sitemap for search engines
```

## 5. Getting Started

Since this is a vanilla static website, no installation (`npm install`, `pip install`, etc.) is required.

Clone or download the repository to your local machine, and you are ready to view or serve the files.

## 6. How to Run the Website

### Method 1: Local Static HTTP Server (Recommended)

Running through a local static server ensures that relative directory URLs (e.g. `about-us/`, `projects/`, `articles/`) resolve identically to a production web server.

You can use any standard static server tool:

- **Using Python 3:**
  ```bash
  python -m http.server 8000
  ```
  Then open `http://localhost:8000` in your web browser.

- **Using Node.js (`npx serve` or `npx http-server`):**
  ```bash
  npx serve .
  ```

- **Using VS Code Live Server extension:**
  Right-click `index.html` and select **Open with Live Server**.

### Method 2: Direct File Inspection

You can directly open `index.html` in any modern web browser (Chrome, Edge, Firefox, Safari).

*Note:* An active internet connection is required to fetch CDN resources (Tailwind CSS, Lenis, Google Fonts Tajawal, and external project imagery).

## 7. Important Files

- `index.html`: Entry point of the website.
- `js/script.js`: Handles mobile navigation toggle, navbar scroll dynamics, Lenis smooth scrolling, scroll-to-top button, dynamic article and project card rendering, project modal lightbox with auto-slider, and WhatsApp quote submission.
- `css/style.css`: Custom CSS variables, floating navbar styling, animations, and custom scrollbar styles.
- `google58051ffbc8570adc.html`: Verification file for Google Search Console ownership. Keep in site root.
- `sitemap.xml` & `robots.txt`: Search engine indexation configurations.

## 8. Additional Notes

- **Google Site Verification:** Preserve `google58051ffbc8570adc.html` in the root directory to maintain active Google Search Console verification.
- **External Image Dependencies:** Project card details load high-resolution project photos hosted on `postimg.cc`.
- **Favicon Reference:** The HTML headers link to `images/icon.png` as the main favicon and `images/logo.png` for article pages.
