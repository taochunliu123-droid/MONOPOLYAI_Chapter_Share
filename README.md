# 🤖 AI Prompt Engineering Monopoly Game

An educational board game that teaches AI prompt engineering concepts through interactive gameplay. Available in Traditional Chinese, English, and Swahili.

## 🎮 Features

- **Multi-language Support**: Traditional Chinese (繁體中文), English, and Kiswahili
- **Educational Content**: Learn about AI prompts, collaboration, tools, and ethics
- **Interactive Gameplay**: Monopoly-style board game with questions and challenges
- **Team-based**: Support for multiple teams with customizable names
- **Dynamic Questions**: Questions loaded from external JSON file for easy updates

## 📁 Project Structure

```
.
├── index.html          # Main game HTML file
├── questions.json      # Questions database (separate for security)
├── vercel.json        # Vercel deployment configuration
├── package.json       # Project metadata
└── README.md          # This file
```

## 🚀 Deploy to Vercel

### Prerequisites

1. Install [Vercel CLI](https://vercel.com/docs/cli):
   ```bash
   npm install -g vercel
   ```

2. Create a Vercel account at [vercel.com](https://vercel.com)

### Deployment Steps

#### Method 1: Using Vercel CLI (Recommended)

1. Navigate to your project directory:
   ```bash
   cd your-project-folder
   ```

2. Login to Vercel:
   ```bash
   vercel login
   ```

3. Deploy your project:
   ```bash
   vercel
   ```

4. Follow the prompts:
   - Set up and deploy? **Y**
   - Which scope? Select your account
   - Link to existing project? **N**
   - What's your project's name? **ai-prompt-monopoly** (or your preferred name)
   - In which directory is your code located? **./**
   - Want to modify settings? **N**

5. Your game will be deployed! Vercel will provide you with a URL.

6. For production deployment:
   ```bash
   vercel --prod
   ```

#### Method 2: Using Vercel Dashboard (Git Integration)

1. Push your code to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit - AI Monopoly Game"
   git remote add origin YOUR_GITHUB_REPO_URL
   git push -u origin main
   ```

2. Go to [Vercel Dashboard](https://vercel.com/dashboard)

3. Click "Add New..." → "Project"

4. Import your GitHub repository

5. Configure project settings:
   - **Framework Preset**: Other
   - **Build Command**: (leave empty)
   - **Output Directory**: (leave empty)
   - **Install Command**: (leave empty)

6. Click "Deploy"

7. Wait for deployment to complete!

### Custom Domain (Optional)

1. Go to your project in Vercel Dashboard
2. Click "Settings" → "Domains"
3. Add your custom domain
4. Follow DNS configuration instructions

## 🔧 Local Development

To test locally, simply open `index.html` in a modern web browser. 

For local server testing:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Using Vercel CLI
vercel dev
```

Then visit `http://localhost:8000` (or the port shown)

## 🎯 Game Instructions

1. **Select Language**: Choose between Traditional Chinese, English, or Kiswahili
2. **Set Rounds**: Choose how many rounds to play (1-20)
3. **Add Teams**: Create teams with custom names
4. **Start Game**: Click "開始遊戲" / "Start Game" / "Anza Mchezo"
5. **Roll Dice**: Take turns rolling dice and moving around the board
6. **Answer Questions**: Land on spaces to answer questions and earn resources
7. **Win**: Team with the most resources at the end wins!

## 📝 Updating Questions

To update or add questions:

1. Edit `questions.json` file
2. Follow the existing JSON structure
3. Deploy updated version to Vercel:
   ```bash
   vercel --prod
   ```

## 🔒 Security Features

- Questions are stored in a separate JSON file (not embedded in HTML)
- Easy to update without modifying main game code
- Prevents easy viewing/copying of questions from page source

## 🌐 Browser Support

- Chrome (recommended)
- Firefox
- Safari
- Edge
- Mobile browsers

## 👤 Author

**Tao Chun Liu (PM Mayors)**
- LinkedIn: [https://www.linkedin.com/in/taochunliu/](https://www.linkedin.com/in/taochunliu/)
- Role: Product Manager specializing in AI and Agile methodologies

## 📄 License

MIT License - Feel free to use and modify for educational purposes

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Add questions in new languages

## 📞 Support

For issues or questions, please:
1. Check the existing documentation
2. Open an issue on GitHub
3. Contact via LinkedIn

---

**里長伯幫助您用AI玩轉敏捷 | Helping you master AI for Agile**
