# Push to GitHub - Quick Guide

## ⚠️ Important: API Keys Are Included

This project includes hardcoded API keys. Once you push to GitHub, your API keys will be public. **You will be responsible for monitoring and regenerating them if needed.**

---

## 🚀 3-Step GitHub Push

### Step 1: Initialize Git
```bash
cd ~/Downloads/market-insight-weekly

git init
git add .
git commit -m "Initial commit: Market Insight Weekly v2.0"
```

### Step 2: Create GitHub Repository

1. Go to https://github.com/new
2. Name: `market-insight-weekly`
3. Description: "AI-powered market intelligence briefing for Hong Kong & Greater China"
4. Choose **Public**
5. Do NOT check "Initialize with README"
6. Click "Create repository"

### Step 3: Push to GitHub
```bash
# Replace YOUR_USERNAME with your GitHub username
git remote add origin https://github.com/YOUR_USERNAME/market-insight-weekly.git
git branch -M main
git push -u origin main
```

Done! Your repo is now live on GitHub. 🎉

---

## ✅ Verify on GitHub

Visit `https://github.com/YOUR_USERNAME/market-insight-weekly` and check:

- ✅ `server.js` - Contains hardcoded API keys
- ✅ `public/index.html` - Frontend
- ✅ `package.json` - Dependencies
- ✅ `README.md` - Documentation
- ✅ `.gitignore` - File protection rules
- ✅ `node_modules/` - Should NOT be visible (protected by .gitignore)

---

## 🔄 If You Need to Update

To update your code after the initial push:

```bash
git add .
git commit -m "Update: [what changed]"
git push
```

---

## 🛡️ Monitoring Your API Keys

Since your keys are public, monitor for unauthorized usage:

**NewsAPI.org:**
- Log into https://newsapi.org
- Check "Usage" dashboard
- Alert: If calls spike beyond your usage, regenerate the key

**WorldNewsAPI:**
- Log into https://www.worldnewsapi.com
- Check "API Usage"
- Alert: Monitor for unusual patterns

**Google Gemini:**
- Log into https://aistudio.google.com
- Check "API Usage"
- Alert: Monitor billing and usage

---

## 🔑 Regenerating Keys (If Exposed)

If you notice suspicious activity:

1. **NewsAPI.org**: Delete old key, generate new one
2. **WorldNewsAPI**: Regenerate API key
3. **Gemini**: Create new API key, delete old one
4. **Update GitHub**: Edit `server.js` with new keys
   ```bash
   git add server.js
   git commit -m "Rotate API keys"
   git push
   ```

---

## 📊 Files Being Shared

| File | Contains | Public? |
|------|----------|---------|
| `server.js` | Hardcoded API keys | ✅ Yes |
| `public/index.html` | Frontend code | ✅ Yes |
| `package.json` | Dependencies | ✅ Yes |
| `.gitignore` | File protection rules | ✅ Yes |
| `node_modules/` | Third-party code | ❌ No (ignored) |

---

## 🎯 What Others See

When someone visits your GitHub repo:

✅ **They can see:**
- Your server code (with API keys)
- How the app works
- How to run it locally
- Full documentation

✅ **They cannot see:**
- `node_modules/` folder
- `.git` internal files
- System files (`.DS_Store`, etc.)

---

## 🚀 Next: Share Your Repo!

Once pushed, share the link:

```
https://github.com/YOUR_USERNAME/market-insight-weekly
```

People can:
1. Clone it: `git clone https://github.com/YOUR_USERNAME/market-insight-weekly.git`
2. Install: `npm install`
3. Run: `npm start`

It just works! No .env setup needed. 🎉

---

## 📝 Common Git Commands

```bash
# Check status
git status

# Add changes
git add .

# Commit
git commit -m "Your message"

# Push to GitHub
git push

# View history
git log

# Revert last commit (if needed)
git revert HEAD
```

---

## ⚡ You're Ready!

Your project is now ready to share publicly. Just follow the 3 steps above and you're done.

**Questions?** Check GitHub's guides at https://docs.github.com
