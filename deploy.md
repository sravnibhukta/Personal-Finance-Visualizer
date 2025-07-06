# 🚀 Deployment Guide

## Deploy to Vercel

### Prerequisites
- Vercel account (free at vercel.com)
- Project code on GitHub (recommended)

### Method 1: GitHub Integration (Recommended)
1. Push your code to GitHub
2. Go to vercel.com and log in
3. Click "New Project"
4. Import your GitHub repository
5. Configure build settings:
   - Build Command: `npm run build`
   - Output Directory: `dist/public`
   - Install Command: `npm install`
6. Click "Deploy"

### Method 2: Vercel CLI
1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy from project directory:
   ```bash
   vercel
   ```

4. Follow the prompts:
   - Set up and deploy? `Y`
   - Which scope? (select your account)
   - Link to existing project? `N`
   - What's your project's name? `personal-finance-visualizer`
   - In which directory is your code located? `./`

### Method 3: Manual Upload
1. Build the project locally:
   ```bash
   npm run build
   ```

2. Upload the `dist` folder contents to Vercel

### Live URL
After deployment, your app will be available at:
```
https://your-app-name.vercel.app
```

### Environment Variables
For production, set these in Vercel dashboard:
- `NODE_ENV=production`

### Troubleshooting
If deployment fails:
1. Check build logs in Vercel dashboard
2. Ensure all dependencies are in `package.json`
3. Verify build command works locally
4. Check `vercel.json` configuration

### Custom Domain
To use a custom domain:
1. Go to project settings in Vercel
2. Add your domain
3. Configure DNS records