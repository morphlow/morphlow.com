# Hello World Website - Astro + Netlify

## Project Overview

This is a basic "hello world" website for **morphlow.com** built using **Astro**, a modern static site generator, and deployed to the web using **Netlify**.

## Technology Stack

- **Framework**: Astro - A lightweight, component-based static site generator
- **Deployment**: Netlify - A modern web hosting platform for static sites and serverless functions
- **Language**: JavaScript/TypeScript with Astro components

## Project Structure

```
morphlow.com/
├── src/
│   ├── pages/
│   │   └── index.astro          # Home page with "hello world" content
│   ├── layouts/
│   │   └── Layout.astro         # Base layout component
│   └── components/
│       └── HelloWorld.astro     # Hello world component
├── public/
│   └── favicon.svg              # Favicon
├── astro.config.mjs             # Astro configuration
├── package.json                 # Project dependencies
└── netlify.toml                 # Netlify configuration
```

## Getting Started

### Prerequisites
- Node.js 18.x or higher
- npm or yarn package manager

### Installation

```bash
npm install
```

### Development

Run the development server:

```bash
npm run dev
```

The site will be available at `http://localhost:3000`

### Build

Create an optimized production build:

```bash
npm run build
```

### Preview

Preview the production build locally:

```bash
npm run preview
```

## Deployment to Netlify

### Option 1: Connect Git Repository (Recommended)

1. Push your repository to GitHub, GitLab, or Bitbucket
2. Go to [Netlify](https://app.netlify.com) and sign up/login
3. Click "New site from Git"
4. Connect your Git provider and select the repository
5. Set the build command to `npm run build`
6. Set the publish directory to `dist`
7. Click "Deploy site"

### Option 2: Manual Deployment

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Build the site
npm run build

# Deploy to Netlify
netlify deploy --prod --dir=dist
```

### Configuration

The `netlify.toml` file contains the deployment configuration:

```toml
[build]
  command = "npm run build"
  publish = "dist"

[dev]
  command = "npm run dev"
  port = 3000
```

## Key Features

- **Fast Performance**: Static site generation ensures optimal speed
- **Component-Based**: Reusable Astro components for maintainability
- **SEO Friendly**: Static HTML output with excellent SEO capabilities
- **Zero JavaScript (by default)**: Ships minimal JS to the browser
- **Easy Deployment**: Simple integration with Netlify for automatic deployments

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Create production build
- `npm run preview` - Preview production build
- `npm run astro ...` - Run Astro CLI commands

## Next Steps

To expand this project:

1. Add more pages in `src/pages/`
2. Create additional components in `src/components/`
3. Add styling with CSS or a CSS framework
4. Connect a headless CMS for content management
5. Add dynamic features with Astro integrations

## Resources

- [Astro Documentation](https://docs.astro.build)
- [Netlify Documentation](https://docs.netlify.com)
- [Astro Integrations](https://astro.build/integrations/)
- [Netlify Deployment Guide](https://docs.netlify.com/integrations/frameworks/astro/)

## License

MIT License - Feel free to use this project as a starting point for your own websites.
