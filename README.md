# Personal Portfolio

Source code for the personal portfolio website of Atharva Kumkar — a photographer and videographer specialising in automotive photography. The site presents individual galleries for each vehicle shoot, a portfolio overview, a wallpapers section, and a contact page. It is a fully static site with no build step, deployed on Netlify.

Live site: https://atharvakumkar.netlify.app

## Table of Contents

- [Pages](#pages)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [Running Locally](#running-locally)
- [Deployment](#deployment)
- [Author](#author)
- [License](#license)

---

## Pages

**Core pages**

| File | Description |
|---|---|
| `mywebsite.html` | Home page; hero section with profile image, intro text, WhatsApp contact button, and a featured gallery grid of three vehicles |
| `portfolio.html` | Full portfolio overview listing all shoot projects |
| `wallpaper.html` | Downloadable automotive wallpapers section |
| `contactpage.html` | Contact form and direct contact links |

**Individual vehicle gallery pages**

| File | Subject |
|---|---|
| `huracan_page.html` / `huracan_page2.html` | Lamborghini Huracan |
| `aventador_page.html` | Lamborghini Aventador |
| `ferrari296_page.html` | Ferrari 296 |
| `mclaren750s_page.html` | McLaren 750S |
| `porschecarrera_page.html` | Porsche Carrera |
| `bmwM3_page.html` | BMW M3 |
| `lexusls300_page2.html` | Lexus LS300 |
| `rangerover_page2.html` | Range Rover Sport Autobiography |
| `harley_page.html` | Harley Davidson |
| `hondacbr_page.html` | Honda CBR |
| `jawa_page.html` | Jawa |

---

## Project Structure

```
Personal-Portfolio/
|
|-- mywebsite.html              # Home page and entry point
|-- portfolio.html              # Portfolio overview
|-- wallpaper.html              # Wallpapers section
|-- contactpage.html            # Contact page
|
|-- huracan_page.html           # Lamborghini Huracan gallery (variant 1)
|-- huracan_page2.html          # Lamborghini Huracan gallery (variant 2)
|-- aventador_page.html         # Lamborghini Aventador gallery
|-- ferrari296_page.html        # Ferrari 296 gallery
|-- mclaren750s_page.html       # McLaren 750S gallery
|-- porschecarrera_page.html    # Porsche Carrera gallery
|-- bmwM3_page.html             # BMW M3 gallery
|-- lexusls300_page2.html       # Lexus LS300 gallery
|-- rangerover_page2.html       # Range Rover Sport gallery
|-- harley_page.html            # Harley Davidson gallery
|-- hondacbr_page.html          # Honda CBR gallery
|-- jawa_page.html              # Jawa gallery
|
|-- assets/                     # Photography assets: images and media files
|-- my-project/                 # Sub-project directory
|-- netlify.toml                # Netlify deployment configuration
|-- .gitattributes
```

---

## Tech Stack

**Markup and Styling**

- HTML5
- Tailwind CSS v4 — loaded via the browser CDN (`@tailwindcss/browser@4`); no build step or PostCSS configuration required
- CSS3 — custom font utility classes for Manrope and Raleway
- Dark mode — implemented via Tailwind's `dark:` variant, inheriting from system preference

**Typography**

- Manrope — body font, loaded from Google Fonts
- Raleway — display font, loaded from Google Fonts

**JavaScript**

- Vanilla JavaScript — single `toggleMenu()` function handles the responsive hamburger navigation on mobile viewports

**Deployment**

- Netlify — static site hosting with configuration defined in `netlify.toml`

---

## Running Locally

The site has no dependencies to install and no build process. Open any HTML file directly in a browser:

```bash
# Clone the repository
git clone https://github.com/Atharvakumkar/Personal-Portfolio.git
cd Personal-Portfolio

# Open the home page
open mywebsite.html        # macOS
start mywebsite.html       # Windows
xdg-open mywebsite.html    # Linux
```

Alternatively, use a local static server to avoid any browser restrictions on local file paths:

```bash
npx serve .
```

Then open `http://localhost:3000/mywebsite.html` in a browser.

---

## Deployment

The site is deployed to Netlify. Any push to the `main` branch triggers an automatic deployment. The `netlify.toml` file at the root contains the deployment configuration.

To deploy a fork manually via the Netlify CLI:

```bash
npm install -g netlify-cli
netlify deploy --prod --dir .
```

---

## Author

Atharva Kumkar

---

## License

This project is released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files, to deal in the software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, and to permit persons to whom the software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
