# Nikolozch Website

Personal website of Nikoloz Chitashvili - Tech writeups, thoughts and ideas.

## Tech Stack

- **Vue.js 3** - Progressive JavaScript framework
- **Vite** - Next-generation frontend build tool
- **Vue Router** - Official router for Vue.js

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or pnpm

### Installation

```bash
npm install
```

### Development

Start the development server with hot reload:

```bash
npm run dev
```

The app will be available at `http://localhost:3000`

### Build for Production

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

## Project Structure

```
nikolozch-website/
├── public/                 # Static assets (copied as-is to dist)
│   ├── images/            # Images and media
│   └── *.css, *.js         # Compiled CSS and JS
├── src/                    # Vue.js source code
│   ├── assets/            # Module assets (processed by Vite)
│   ├── components/        # Reusable Vue components
│   ├── router/           # Vue Router configuration
│   ├── styles/           # Global CSS styles
│   ├── views/            # Page components
│   ├── App.vue           # Root component
│   └── main.js           # Application entry point
├── index.html             # HTML entry point
├── package.json           # Dependencies and scripts
├── vite.config.js         # Vite configuration
└── README.md              # This file
```

## Features

- Static blog with Hack The Box writeups
- Responsive design
- Fast HMR (Hot Module Replacement) during development
- SEO-friendly structure

## License

ISC
