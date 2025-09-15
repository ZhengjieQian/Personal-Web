# Development Setup Guide

## Quick Start

1. **Install Node.js** (if not already installed):
   - Download from https://nodejs.org/
   - Choose the LTS version

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Start development server**:
   ```bash
   npm run dev
   ```

This will:
- Compile SCSS to CSS automatically when you make changes
- Start a live server that auto-refreshes the browser
- Open your website at http://localhost:3000

## Available Commands

- `npm run dev` - Start development server with auto-reload
- `npm run watch-scss` - Only watch and compile SCSS files
- `npm run serve` - Only start the live server
- `npm run build` - Build production CSS (compressed)

## How It Works

- **SCSS Compilation**: Automatically compiles `scss/custom.scss` to `css/custom.css`
- **Live Reload**: Browser automatically refreshes when you save HTML, CSS, or SCSS files
- **Port**: Website runs on http://localhost:3000

## File Structure

- Edit `index.html` for HTML changes
- Edit `scss/custom.scss` for styling changes
- The compiled CSS will be automatically generated in `css/custom.css`

## Troubleshooting

If you get permission errors on Windows:
```bash
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
```

Then try `npm install` again.
