# Basketball Camp Website - Maintenance Guide

## 🏀 Website Information
- **Live Website:** https://brilliant-figolla-9de223.netlify.app/
- **GitHub Repository:** https://github.com/sabeertj/basketball-camp-site
- **Auto-Deploy:** Any changes to the `main` branch automatically update the live website

---

## 📝 Quick Content Updates (No Technical Skills Required)

### Method 1: Edit Directly on GitHub (Easiest)

**Step 1: Go to Your Repository**
- Visit: https://github.com/sabeertj/basketball-camp-site
- Make sure you're logged into GitHub

**Step 2: Edit the Website**
- Click on `index.html`
- Click the pencil icon (✏️) in the top right
- Make your changes (see common updates below)
- Scroll to bottom and add a commit message like "Update camp dates"
- Click "Commit changes"
- Wait 1-2 minutes for the website to automatically update

### Common Content Updates

#### Update Camp Information
Find and change these sections in `index.html`:

**Camp Name:**
```html
<h1>🏀 Elite Basketball Camp</h1>
<!-- Change to your camp name -->
<h1>🏀 Your Camp Name Here</h1>
```

**Camp Dates and Details:**
```html
<strong>Ages:</strong> 8-16 years old<br>
<strong>Duration:</strong> 5 days<br>
<strong>Time:</strong> 9:00 AM - 3:00 PM<br>
<strong>Location:</strong> Local High School Gym
```

**Contact Information:**
```html
<p>📧 Email: info@basketballcamp.com</p>
<p>📞 Phone: (555) 123-4567</p>
<p>📍 Location: Your City, State</p>
```

**UCSF Fundraising Link:**
```html
<a href="https://giving.ucsf.edu/fund/your-specific-fund-link" class="donate-button" target="_blank">
```

---

## 📸 Adding Photos

### Step 1: Upload Photos to GitHub
1. Go to https://github.com/sabeertj/basketball-camp-site
2. Click on `images` folder → `camp-photos` folder
3. Click "Add file" → "Upload files"
4. Drag your photos into the upload area
5. Name them clearly (e.g., `skills-training-2024.jpg`, `team-photo.jpg`)
6. Add commit message: "Add new camp photos"
7. Click "Commit changes"

### Step 2: Display Photos on Website
1. Edit `index.html` (pencil icon)
2. Find the photo placeholder section:
```html
<div class="photo-placeholder">📸 Camp Action Shot 1</div>
```
3. Replace with:
```html
<div class="photo-item">
    <img src="images/camp-photos/your-photo-name.jpg" alt="Camp Action Shot">
    <div class="photo-caption">Your photo description</div>
</div>
```
4. Commit changes

---

## 🎥 Adding Videos

### Step 1: Upload to YouTube
1. Upload your camp videos to YouTube
2. Copy the video ID from the URL
   - Example: `https://youtube.com/watch?v=ABC123DEF456`
   - Video ID: `ABC123DEF456`

### Step 2: Add to Website
1. Edit `index.html`
2. Find video placeholder:
```html
<div class="video-placeholder">🎥 Camp Highlight Reel</div>
```
3. Replace with:
```html
<div class="video-item">
    <iframe src="https://www.youtube.com/embed/ABC123DEF456" allowfullscreen></iframe>
    <div class="video-title">Camp Highlight Reel</div>
</div>
```
4. Commit changes

---

## 💻 Advanced Updates (For Technical Users)

### Method 2: Clone Repository and Work Locally

**Step 1: Clone Repository**
```bash
git clone https://github.com/sabeertj/basketball-camp-site.git
cd basketball-camp-site
```

**Step 2: Create a New Branch**
```bash
# Create branch for your updates
git checkout -b update-camp-content

# Make your changes to files
# Add photos to images/camp-photos/
# Edit index.html
```

**Step 3: Commit and Push Changes**
```bash
git add .
git commit -m "Update camp content and add new photos"
git push origin update-camp-content
```

**Step 4: Create Pull Request**
1. Go to https://github.com/sabeertj/basketball-camp-site
2. GitHub will show "Compare & pull request" button
3. Add description of changes
4. Click "Create pull request"
5. Click "Merge pull request" to make changes live

---

## 🔄 Website Update Workflow

### For Small Changes (Text updates, contact info)
**GitHub Web Interface** → Edit `index.html` → Commit → Auto-deploy (2 minutes)

### For Major Updates (New photos, videos, redesign)
**Local Development** → Create branch → Make changes → Push → Pull Request → Merge

---

## 📁 File Structure Reference

```
basketball-camp-site/
├── index.html                 # Main website file (edit this for content)
├── images/
│   ├── camp-photos/          # Upload camp photos here
│   ├── backgrounds/          # Background images
│   └── logos/               # Camp logos
└── README.md                # This guide
```

---

## 🆘 Common Issues & Solutions

### Website Not Updating?
- Wait 2-3 minutes after committing changes
- Check Netlify deploy status: https://app.netlify.com/
- Make sure you committed to the `main` branch

### Photo Not Showing?
- Check file name spelling matches exactly
- Ensure photo is uploaded to correct folder: `images/camp-photos/`
- File names are case-sensitive

### Video Not Playing?
- Make sure video is public on YouTube
- Use the correct video ID in embed code
- Check that iframe code is complete

---

## 📞 Getting Help

### Quick Fixes
1. **Undo Last Change:** Go to repository → Click "commits" → Find your change → Click "Revert"
2. **Start Over:** Download a fresh copy from GitHub

### Need Technical Help?
- Check GitHub repository issues: https://github.com/sabeertj/basketball-camp-site/issues
- Review commit history to see what changed
- Compare with working versions

---

## ✅ Pre-Season Website Checklist

**Content Updates:**
- [ ] Update camp dates and times
- [ ] Update registration information
- [ ] Update contact information
- [ ] Update UCSF fundraising link
- [ ] Add new staff photos/bios

**Media Updates:**
- [ ] Upload new camp photos
- [ ] Create highlight video for YouTube
- [ ] Update hero background image
- [ ] Add camp logo

**Testing:**
- [ ] Check website on mobile phone
- [ ] Test all links (especially donation link)
- [ ] Verify contact information is correct
- [ ] Check that videos play properly

---

## 🎯 Quick Reference

| Task | Method | Time |
|------|--------|------|
| Update camp dates | GitHub web edit | 2 minutes |
| Add 5 photos | Upload to GitHub + edit HTML | 10 minutes |
| Add video | YouTube upload + edit HTML | 15 minutes |
| Major redesign | Clone repo + branch workflow | 1+ hours |

**Remember:** Every change to the `main` branch automatically updates your live website at https://brilliant-figolla-9de223.netlify.app/ within 1-2 minutes!
