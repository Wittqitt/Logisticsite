# GitHub Setup Instructions

## After creating your GitHub repository, run these commands:

1. Add the remote repository (replace YOUR_USERNAME and REPO_NAME):
   ```
   git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
   ```

2. Push your code:
   ```
   git push -u origin SOURCECODE:main
   ```

   OR if you want to rename the branch first:
   ```
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
   git push -u origin main
   ```

## Then connect to Netlify:

1. Go to https://app.netlify.com
2. Click "Add new site" → "Import an existing project"
3. Choose "GitHub"
4. Authorize Netlify to access GitHub
5. Select your repository
6. Configure build settings:
   - Build command: (leave empty for static site)
   - Publish directory: / (root)
7. Click "Deploy site"

After this, Netlify will automatically deploy every time you push to GitHub!

