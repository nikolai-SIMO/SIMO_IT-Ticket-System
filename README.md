# SIMO IT Ticket System - Outlook Add-in

This repository hosts the SIMO IT Support Ticket submission system for Outlook.

## 📁 Repository Structure

Your repository should contain these files:

```
SIMO_IT-Ticket-System/
├── index.html          ← Main HTML file (loads the Microsoft Form)
├── manifest.xml        ← Outlook add-in manifest
├── icon16.png         ← 16x16px icon
├── icon32.png         ← 32x32px icon
├── icon80.png         ← 80x80px icon
└── README.md          ← This file
```

## 🎨 Creating the Icon Files

You need to create three PNG icon files with your SIMO logo:

### Option 1: Use Your Existing SIMO Logo
1. Open your SIMO logo in an image editor (Photopea, Photoshop, GIMP, etc.)
2. Create three versions:
   - **icon16.png**: 16x16 pixels
   - **icon32.png**: 32x32 pixels
   - **icon80.png**: 80x80 pixels
3. Save as PNG with transparent background
4. Upload to the root of this repository

### Option 2: Use Placeholder Icons (Quick Start)
If you want to test quickly, you can use these placeholder icon URLs temporarily:
- Download any simple icon from https://www.flaticon.com/ (free with attribution)
- Resize to 16x16, 32x32, and 80x80 pixels
- Name them exactly as shown above

## 🚀 Setup Instructions

### Step 1: Upload Files to GitHub
1. Upload all files from the `/mnt/user-data/outputs/` folder to your repository
2. Make sure the files are in the root directory (not in a subfolder)

### Step 2: Enable GitHub Pages
1. Go to repository Settings
2. Click "Pages" in the left sidebar
3. Under "Source", select "main" branch
4. Click "Save"
5. Your site will be published at: `https://nikolai-simo.github.io/SIMO_IT-Ticket-System/`

### Step 3: Test the Page
1. Wait 1-2 minutes for GitHub Pages to deploy
2. Visit: `https://nikolai-simo.github.io/SIMO_IT-Ticket-System/`
3. You should see the IT ticket form load

### Step 4: Deploy the Outlook Add-in
1. Go to Microsoft 365 Admin Center → Integrated apps
2. Click "Upload custom apps"
3. Select "Office Add-in"
4. Choose "Provide link to manifest file"
5. Enter: `https://nikolai-simo.github.io/SIMO_IT-Ticket-System/manifest.xml`
6. Click "Validate" then "Next"
7. Assign to users and deploy

## 📝 Form URL

The form is hosted at:
```
https://forms.office.com/Pages/ResponsePage.aspx?id=aWc9G88WnEO78pAi4oGmGoalILOG8DhOpLKcY7DksvVUNUsJWThNRDNUUlhPT0ZDWEUwRlR8TU1ZSy4u
```

If you need to update the form URL, edit the `src` attribute in `index.html`.

## 🔧 Troubleshooting

**GitHub Pages not loading?**
- Check that files are in the root directory
- Wait 5-10 minutes after enabling Pages
- Check Settings → Pages for deployment status

**Manifest validation errors?**
- Ensure all icon files exist and are accessible
- Check that GitHub Pages is enabled and deployed
- Verify the manifest.xml file is in the root directory

**Form not loading in Outlook?**
- Check browser console for CORS errors
- Ensure you're signed into Microsoft 365
- Try loading the form directly in a browser first

## 📞 Support

For issues or questions, contact: IT-SIMO - Nikolai Nöthling

---

**Created:** October 2025  
**Version:** 1.0.0
