# Jacob Thomas Khalil — Art Portfolio

A minimal, responsive art portfolio for showcasing photography, illustration, poetry, painting, and fashion. Built with accessibility, performance, and elegance in mind.

## Live Site
[https://jacobthomaskhalil.net](https://jacobthomaskhalil.net)

## Features

- Responsive layout optimized for mobile and desktop
- Lazy-loaded images in modern WebP format
- Fancybox gallery integration for immersive image viewing
- Font Awesome icons
- Animated hamburger navigation
- Video support for digital and printed works
- Modular CSS and JS structure
- ARIA accessibility compliance

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Fancybox v4 (for lightbox functionality)
- Font Awesome (icons)
- PageSpeed & Lighthouse optimization techniques

## Project Structure

├── index.html
├── fashion/
│   └── index.html
├── illustration/
│   └── index.html
├── painting/
│   └── index.html
├── photography/
│   └── index.html
├── poetry/
│   └── index.html
├── assets/
│   ├── fonts/
│   ├── images/
│   │   ├── headers/
│   │   ├── icon.png
│   │   ├── fashion/
│   │   ├── illustration/
│   │   ├── painting/
│   │   ├── photography/
│   │   └── poetry/
│   ├── styles/
│   ├── scripts/
│   └── video/
├── README.md


## Tech Stack

- HTML5 / CSS3 / JavaScript (vanilla)
- [Fancybox v4](https://fancyapps.com/fancybox/)
- Font Awesome (self-hosted)
- Responsive images with `<picture>` + `srcset`
- Page transitions and accessibility enhancements

## PageSpeed Results

| Metric              | Desktop | Mobile |
|---------------------|---------|--------|
| **Performance**     | 100     | 93     |
| **Accessibility**   | 100     | 100    |
| **Best Practices**  | 100     | 100    |
| **SEO**             | 100     | 100    |

- **Mobile performance deductions** were due to:
  - Slight image oversizing (`hero-header2_800.webp` loaded at larger-than-displayed resolution)
  - Render-blocking CSS (non-critical styles like Font Awesome or Hamburger.css)
  - Moderate Cumulative Layout Shift (CLS) caused by late-rendered hero text

## Optimization Notes

- Images use `width` & `height` attributes to minimize layout shifts
- Preload is used selectively for critical images
- JS is deferred
- CSS is modularized to only load what's necessary on each page
