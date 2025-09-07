# Build Process Documentation

## Overview
This project now uses Vite to build the React/TypeScript application for deployment to GitHub Pages.

## Build Commands

### Development
```bash
npm run dev
```
Starts the development server at http://localhost:5173/justthetipbot/

### Production Build
```bash
npm run build
```
Builds the application to the `dist/` directory with optimized, production-ready assets.

### Preview Build
```bash
npm run preview
```
Previews the production build locally.

## GitHub Pages Deployment

The project is configured to automatically build and deploy to GitHub Pages when changes are pushed to the main branch.

### Automatic Deployment
- GitHub Actions workflow (`.github/workflows/deploy.yml`) automatically builds and deploys the site
- Build artifacts are generated in the `dist/` folder
- GitHub Pages serves the compiled static files from the `dist/` folder

### Manual Deployment
```bash
npm run deploy
```
This command will build the project and deploy it using gh-pages package.

## Project Structure

```
├── index.html          # Main HTML template
├── index.tsx           # React application entry point
├── App.tsx             # Main React component
├── components/         # React components
├── vite.config.ts      # Vite configuration
├── tsconfig.json       # TypeScript configuration
├── dist/               # Build output (generated, not committed)
└── .github/workflows/  # GitHub Actions workflows
```

## Configuration

- **Base URL**: `/justthetipbot/` (configured for GitHub Pages)
- **Build Tool**: Vite with React plugin
- **Output Directory**: `dist/`
- **TypeScript**: Enabled with strict mode

## Environment Variables

The build process supports environment variables:
- `GEMINI_API_KEY`: API key for Gemini integration (optional)

These are defined in the Vite configuration and can be set in your environment or `.env` file.