# Simple Deployment Guide

## Quick Fix for Vercel Deployment

The build process is timing out due to the large number of dependencies. Here are alternative deployment approaches:

### Option 1: Deploy Frontend Only (Recommended)
Since this app uses in-memory storage, deploy just the frontend as a static site:

1. **Build frontend only:**
   ```bash
   cd client
   vite build
   ```

2. **Deploy to Netlify (Free):**
   - Go to netlify.com
   - Drag and drop the `dist` folder
   - Your app will be live instantly

### Option 2: Use Replit Hosting
Since you're already on Replit:
1. Click "Deploy" in Replit
2. Choose "Static Site" 
3. Set build command: `cd client && vite build`
4. Set output directory: `client/dist`

### Option 3: Manual Vercel Deploy
1. Build locally:
   ```bash
   cd client
   npm install
   vite build
   ```

2. Upload `dist` folder to Vercel manually

### Option 4: GitHub + Netlify
1. Push code to GitHub
2. Connect GitHub to Netlify
3. Set build command: `cd client && vite build`
4. Set publish directory: `client/dist`

## Why This Approach Works
- The app uses in-memory storage (no database needed)
- All data is pre-seeded with sample transactions
- Frontend works completely standalone
- No server-side code needed for demo

## Live Demo Features
Once deployed, your app will have:
- Sample transactions and categories
- Working budget management
- All visualizations and charts
- Fully functional UI

Choose the option that works best for you!