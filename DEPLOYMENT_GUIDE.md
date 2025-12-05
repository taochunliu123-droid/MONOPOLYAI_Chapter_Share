# 🚀 Quick Deployment Guide to Vercel

## Files You Need

All files are ready in your download:
- ✅ index.html (game file with footer)
- ✅ questions.json (questions database - hidden from HTML)
- ✅ vercel.json (deployment config)
- ✅ package.json (project metadata)
- ✅ .gitignore (for git repositories)
- ✅ README.md (full documentation)

## Fastest Deployment Method

### Option 1: Drag & Drop (Easiest!)

1. Go to [vercel.com](https://vercel.com)
2. Sign up/Login with GitHub, GitLab, or Bitbucket
3. Click "Add New..." → "Project"
4. Click "Browse" or drag your project folder
5. Done! Your game is live in seconds! 🎉

### Option 2: Using Vercel CLI

```bash
# Install Vercel CLI (one-time setup)
npm install -g vercel

# Navigate to your project folder
cd your-project-folder

# Login to Vercel
vercel login

# Deploy!
vercel

# For production
vercel --prod
```

## What's Special About This Setup?

### ✅ Questions are Hidden
- Questions are in `questions.json` (separate file)
- Not visible in HTML source code
- Harder for users to cheat by viewing source
- Easy to update without touching game code

### ✅ Fixed Footer
- Footer text: "里長伯幫助您用AI玩轉敏捷 | Provided by Tao Chun Liu (PM Mayors)"
- Links to: https://www.linkedin.com/in/taochunliu/
- **Never changes regardless of language selection**
- Always visible at bottom of screen

## Testing Locally First

Before deploying, test locally:

```bash
# Option 1: Python (if installed)
python -m http.server 8000

# Option 2: Node.js
npx http-server

# Option 3: Just open index.html in browser
# (might have CORS issues with questions.json)
```

Visit: `http://localhost:8000`

## After Deployment

You'll get a URL like:
- `https://your-project-name.vercel.app`
- Or your custom domain if configured

### Share Your Game!
- The URL is public and shareable
- Works on mobile and desktop
- No installation needed for players

## Updating the Game

### To Update Questions:
1. Edit `questions.json` locally
2. Run `vercel --prod` to deploy changes
3. Questions update automatically!

### To Update Game:
1. Edit `index.html` locally
2. Run `vercel --prod` to deploy
3. Game updates instantly!

## Important Notes

✅ **All languages work**: Traditional Chinese, English, Swahili  
✅ **Footer always shows**: Your branding is protected  
✅ **Questions hidden**: More secure gameplay  
✅ **Mobile-friendly**: Works on all devices  
✅ **Fast loading**: Optimized for performance  

## Troubleshooting

### Questions not loading?
- Make sure `questions.json` is in same folder as `index.html`
- Check browser console for errors (F12)

### Deployment failed?
- Check all files are in the root directory
- Make sure you're logged into Vercel
- Try `vercel --debug` for more info

### Footer not showing?
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Check if CSS is loading properly

## Need Help?

1. Check README.md for detailed instructions
2. Visit [Vercel Documentation](https://vercel.com/docs)
3. Contact via LinkedIn: https://www.linkedin.com/in/taochunliu/

---

**Good luck with your deployment! 加油！🚀**

里長伯幫助您用AI玩轉敏捷
