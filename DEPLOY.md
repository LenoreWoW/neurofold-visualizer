# Deploy to Netlify - Quick Guide

Your project is ready to deploy! Choose one of these methods:

## Method 1: Netlify CLI (Fastest)

1. Run this command in your terminal:
   ```bash
   netlify deploy --prod --dir=dist
   ```

2. Follow the prompts:
   - Log in to Netlify (browser will open)
   - Choose "Create & configure a new project"
   - Enter a site name (or leave blank for random name)
   - Confirm deployment

3. Your site will be live at: `https://your-site-name.netlify.app`

## Method 2: Netlify Drag & Drop (No Auth Needed)

1. Go to: https://app.netlify.com/drop
2. Drag the `dist` folder into the browser window
3. Done! You'll get a live URL instantly

## Method 3: Connect GitHub (Best for Continuous Deployment)

1. Create a new GitHub repository for this project
2. Push your code:
   ```bash
   git remote remove origin
   git remote add origin https://github.com/YOUR-USERNAME/logfold-visualizer.git
   git push -u origin master
   ```
3. Go to: https://app.netlify.com/start
4. Connect your GitHub repository
5. Deployment will be automatic on every push!

---

**Build command:** `npm run build`
**Publish directory:** `dist`

**Note:** This app runs entirely in the browser with local inference - no API keys or environment variables needed!
