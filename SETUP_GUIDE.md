# 🚀 Quick Setup Guide - Farm & Filter Dashboard

## Step-by-Step Instructions for Deployment

### OPTION 1: Run Locally (Fastest Way to Test)

#### Step 1: Prepare Your Environment
1. Open your terminal/command prompt
2. Navigate to the folder containing these files:
   ```bash
   cd path/to/your/folder
   ```

#### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

#### Step 3: Run the App
```bash
streamlit run app.py
```

#### Step 4: View Your Dashboard
- Your browser should automatically open to `http://localhost:8501`
- If not, copy the URL from the terminal and paste it into your browser

---

### OPTION 2: Deploy to Streamlit Cloud (Free & Public)

#### Prerequisites
- A GitHub account (free at github.com)
- A Streamlit Community Cloud account (free at share.streamlit.io)

#### Step 1: Create GitHub Repository

1. **Go to GitHub** (github.com)
2. **Sign in** to your account
3. Click the **"+"** icon (top right) → **"New repository"**
4. **Name your repository**: `farm-filter-dashboard` (or any name you like)
5. Select **"Public"**
6. **DO NOT** check "Add a README file" (we already have one)
7. Click **"Create repository"**

#### Step 2: Upload Files to GitHub

**EASIEST METHOD - Drag & Drop:**

1. On your new repository page, you'll see: *"Quick setup — if you've done this kind of thing before"*
2. Below that, click: **"uploading an existing file"** link
3. **Drag and drop** ALL these files into the upload area:
   - `app.py`
   - `farm_filter_customer_data.csv`
   - `requirements.txt`
   - `README.md`
   - `.gitignore` (optional)
4. Scroll down and click **"Commit changes"** (green button)

**ALTERNATIVE METHOD - Using Git Commands:**

```bash
# In your project folder, run these commands:
git init
git add .
git commit -m "Initial commit - Farm & Filter Dashboard"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/farm-filter-dashboard.git
git push -u origin main
```
*Replace YOUR_USERNAME with your actual GitHub username*

#### Step 3: Deploy on Streamlit Cloud

1. **Go to** [share.streamlit.io](https://share.streamlit.io)
2. Click **"Sign in with GitHub"**
3. **Authorize** Streamlit to access your GitHub account
4. Click **"New app"** (top right)
5. **Fill in the form:**
   - **Repository**: Select your repository (e.g., `YOUR_USERNAME/farm-filter-dashboard`)
   - **Branch**: `main`
   - **Main file path**: `app.py`
   - **App URL** (optional): Choose a custom URL or use auto-generated
6. Click **"Deploy!"** (red button)

#### Step 4: Wait for Deployment
- Deployment typically takes **2-5 minutes**
- You'll see a progress indicator
- Once done, your app will be live!

#### Step 5: Share Your Dashboard
- Your app URL will be: `https://YOUR_USERNAME-farm-filter-dashboard-HASH.streamlit.app`
- Share this URL with anyone!
- App will auto-update whenever you push changes to GitHub

---

## 🐛 Troubleshooting

### Issue: "Module not found" error
**Solution**: Make sure `requirements.txt` is uploaded and contains all dependencies

### Issue: "File not found" error for CSV
**Solution**: Ensure `farm_filter_customer_data.csv` is in the same directory as `app.py`

### Issue: App crashes on startup
**Solution**: 
1. Check Streamlit Cloud logs (click "Manage app" → "Logs")
2. Verify all files are uploaded correctly
3. Ensure no syntax errors in `app.py`

### Issue: Charts not displaying
**Solution**: Make sure Plotly is listed in `requirements.txt`

### Issue: Slow performance
**Solution**: 
- Filters are working correctly - performance may vary with data size
- Consider reducing data size for faster loading

---

## 📁 File Checklist

Before deploying, make sure you have:
- ✅ `app.py` (Main application)
- ✅ `farm_filter_customer_data.csv` (Data file)
- ✅ `requirements.txt` (Dependencies)
- ✅ `README.md` (Documentation)
- ✅ `.gitignore` (Optional, but recommended)

---

## 🎯 What to Do After Deployment

1. **Test all filters** to ensure they work correctly
2. **Check all visualizations** are displaying properly
3. **Try the download feature** to export data
4. **Share your dashboard link** with your team/instructor
5. **Update the README** with your live app URL

---

## 💡 Tips for Success

- **Use clear commit messages** when updating your GitHub repository
- **Test locally first** before deploying to Streamlit Cloud
- **Monitor the logs** in Streamlit Cloud if something goes wrong
- **Keep dependencies minimal** - only include what you need
- **Update regularly** - Your app auto-updates with GitHub pushes

---

## 🔗 Useful Links

- **Streamlit Documentation**: https://docs.streamlit.io
- **Streamlit Community Cloud**: https://share.streamlit.io
- **Plotly Documentation**: https://plotly.com/python/
- **GitHub Help**: https://docs.github.com

---

## 📧 Need More Help?

1. Check the main README.md for detailed information
2. Review Streamlit's official documentation
3. Search Streamlit Community Forums: https://discuss.streamlit.io
4. Check GitHub repository issues section

---

**Good luck with your deployment! 🚀**
