# ICC1-BritEdge-assignment-static-web

A static, single-page website for the fictional company **BritEdge Solutions Ltd.**, built for use as a capstone project when hosting a static website (e.g. GitHub Pages, Azure Storage static website hosting, AWS S3, Netlify, or similar).

The site is plain HTML/CSS/JS with no build step: styling comes from the Tailwind CSS CDN, and page navigation (Home, About Us, Services, Manufacturing, Logistics, Case Studies, Careers, Contact Us) is handled client-side by showing and hiding sections based on the URL hash.

## Project structure

```
.
├── index.html      Main site (all sections/pages live in this one file)
├── 404.html        Custom "page not found" page
├── favicon.ico     Site favicon
├── images/         Photos used throughout the site
└── README.md
```

## Images

| File | Used for |
|---|---|
| `britedge-manufacturing-facility.jpg` | Home page hero image |
| `britedge-team-meeting.jpg` | About Us — team photo |
| `britedge-precision-engineering.jpg` | Services — manufacturing solutions |
| `britedge-warehouse-logistics.jpg` | Services — logistics & supply chain |
| `britedge-robotic-manufacturing.jpg` | Manufacturing Capabilities page banner |
| `britedge-global-logistics.jpg` | Logistics Solutions page banner |

All photos are from Unsplash and are free to use commercially without attribution under the [Unsplash License](https://unsplash.com/license).

## Running locally

No build tools or dependencies are required. Either:

- Open `index.html` directly in a browser, or
- Serve the folder with any static file server, e.g.:

  ```
  python3 -m http.server 8000
  ```

  then visit `http://localhost:8000`.

## Deploying

Because this is a fully static site (no server-side code), it can be deployed to any static hosting provider by uploading the contents of this folder as-is — for example GitHub Pages, Azure Storage static website hosting, AWS S3 + CloudFront, Netlify, or Vercel. Make sure `404.html` is configured as the custom error/not-found document if your host supports it.

## Notes

This is placeholder/demo content for a fictional company, intended for coursework use rather than production deployment. The contact form does not submit anywhere (there is no backend) — wiring it up to a real endpoint would be a good next step if extending this project.
