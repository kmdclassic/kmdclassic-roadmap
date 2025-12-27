# Komodo Classic Roadmap

A beautiful vertical timeline roadmap website for Komodo Classic (KMDCL) built with Eleventy.

## Features

- Vertical timeline design showing completed and upcoming milestones
- Responsive layout that works on all devices
- Dark theme with Komodo Classic color scheme
- Professional English content written for technical audiences

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Build the site:
```bash
npm run build
```

3. Serve locally (with auto-reload):
```bash
npm run serve
```

The site will be available at `http://localhost:8080`

## Project Structure

```
.
├── src/
│   ├── _data/
│   │   └── roadmap.json      # Roadmap milestones data
│   ├── _layouts/
│   │   └── base.njk          # Base layout template
│   ├── _includes/            # Reusable components
│   ├── assets/
│   │   └── logo.png          # Komodo Classic logo
│   ├── css/
│   │   └── style.css         # Main stylesheet
│   └── index.html            # Main page
├── docs/                      # Generated site (after build) - used for GitHub Pages
├── .eleventy.js              # Eleventy configuration
└── package.json
```

## Customization

To update roadmap milestones, edit `src/_data/roadmap.json`. Each milestone should have:
- `id`: Unique identifier
- `title`: Milestone title
- `date`: Date or time period
- `status`: "completed" or "upcoming"
- `description`: Detailed description
- `links`: Array of related links (optional)
- `blockNumber`: Block number if applicable (optional)

## Deployment

After building (`npm run build`), the `docs/` folder contains the static site ready for deployment. For GitHub Pages, the site is automatically deployed from the `docs/` folder.

