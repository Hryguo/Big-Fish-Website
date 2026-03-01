# Big Fish Chinese Cafe - Website Setup Guide

## 🎉 Your website is ready! Here's what to do next:

---

## STEP 1: Download Images from Your Current Site

Since I can't download images directly, you'll need to save them from your current Wix site. Here's the easy way:

### Method 1: Right-click and save (Easiest)
1. Go to your current website: bigfishchinesecafe.com
2. Right-click on each image → "Save image as..."
3. Save them with these exact names in the `images` folder:

**Required images:**
- `logo.jpg` - Your Big Fish logo (from top of page)
- `hero.jpg` - The main food image at the top
- `menu1.jpg` - First menu image
- `menu2.jpg` - Second menu image
- `dish1.jpg` through `dish9.jpg` - All the food photos from gallery

### Method 2: Download from Wix editor (Alternative)
1. Log into your Wix editor
2. Go to Media Manager
3. Download all images
4. Rename them according to the list above

### Also needed:
- `menu.pdf` - Your menu PDF file (place in main folder next to index.html)

---

## STEP 2: Choose a Hosting Provider

### Option A: Netlify (RECOMMENDED - FREE & EASIEST)

**Why Netlify:**
- ✅ Completely free
- ✅ Super easy drag-and-drop
- ✅ Automatic HTTPS (secure)
- ✅ Fast global CDN

**How to set up:**
1. Go to https://www.netlify.com
2. Click "Sign up" (use your email or GitHub)
3. Click "Add new site" → "Deploy manually"
4. Drag the entire `bigfish-website` folder into the upload area
5. Done! You'll get a URL like `your-site.netlify.app`

**To use your domain (bigfishchinesecafe.com):**
1. In Netlify, go to "Domain settings"
2. Click "Add custom domain"
3. Enter: bigfishchinesecafe.com
4. Follow their instructions to update your DNS settings

---

### Option B: Vercel (Also FREE & Easy)

1. Go to https://vercel.com
2. Sign up with email or GitHub
3. Click "Add New" → "Project"
4. Upload your website folder
5. Follow similar domain setup as Netlify

---

### Option C: GitHub Pages (FREE but requires GitHub)

1. Create a GitHub account if you don't have one
2. Create a new repository
3. Upload all your files
4. Go to Settings → Pages
5. Enable GitHub Pages
6. Your site will be at: username.github.io/repository-name

---

## STEP 3: Point Your Domain

You need to update your domain DNS settings to point to your new hosting:

### If using Netlify:
1. Log into where you bought bigfishchinesecafe.com (GoDaddy, Namecheap, etc.)
2. Find "DNS Settings" or "Manage DNS"
3. Add these records (Netlify will give you exact values):
   - Type: A Record
   - Host: @
   - Points to: (Netlify's IP address)
   
   - Type: CNAME
   - Host: www
   - Points to: (your-site.netlify.app)

4. Wait 15-60 minutes for DNS to update

### If using other hosting:
- They will provide specific DNS instructions
- Usually it's just changing the "A Record" to point to their servers

---

## STEP 4: Update and Customize (Optional)

### To change colors:
Open `css/style.css` and edit these lines at the top:
```css
:root {
    --primary-color: #d32f2f;  /* Main red color */
    --secondary-color: #c62828;  /* Darker red */
    --dark: #1a1a1a;  /* Text color */
}
```

### To change text:
Open `index.html` and edit the text directly. It's all plain English!

### To add more photos:
1. Add image files to the `images` folder
2. Edit `index.html` in the gallery section
3. Add a new div like this:
```html
<div class="gallery-item">
    <img src="images/your-new-photo.jpg" alt="Description">
</div>
```

---

## STEP 5: Cancel Wix

Once your new site is live and working:
1. Log into Wix
2. Go to Settings → Premium Plan
3. Cancel your subscription
4. Save $20-35/month! 💰

---

## 📱 Features Included

✅ Mobile responsive (looks great on phones)
✅ Fast loading
✅ SEO optimized
✅ Google Maps integration
✅ Click-to-call phone numbers
✅ Direct link to online ordering
✅ Social media links
✅ Professional design

---

## 🆘 Need Help?

### Common Issues:

**Images not showing?**
- Make sure image filenames match exactly (case-sensitive!)
- Check that images are in the `images` folder

**Site looks broken?**
- Make sure all three folders are uploaded: css, js, images
- Check that `index.html` is in the root folder

**Domain not working?**
- DNS changes take 15 minutes to 48 hours
- Double-check DNS settings match hosting provider's instructions
- Clear your browser cache

---

## 📊 File Structure

Your website folder should look like this:
```
bigfish-website/
├── index.html          (Main website file)
├── menu.pdf            (Your menu PDF)
├── css/
│   └── style.css       (All styling)
├── js/
│   └── script.js       (Interactive features)
└── images/
    ├── logo.jpg
    ├── hero.jpg
    ├── menu1.jpg
    ├── menu2.jpg
    └── dish1.jpg - dish9.jpg
```

---

## 🎯 Next Steps

1. [ ] Download all images from current site
2. [ ] Sign up for Netlify (or another host)
3. [ ] Upload website folder
4. [ ] Test the site works
5. [ ] Point your domain
6. [ ] Wait for DNS to update
7. [ ] Cancel Wix
8. [ ] Celebrate! 🎉

---

## 💡 Pro Tips

- **Backup**: Keep a copy of all files on your computer
- **Updates**: To update the site, just edit the files and re-upload
- **Analytics**: Add Google Analytics by pasting code before `</body>` in index.html
- **Performance**: Compress images before uploading (use tinypng.com)
- **Mobile testing**: Test on your phone before going live

---

## Cost Comparison

**Before (Wix):** $16-35/month = $192-420/year
**After (Netlify/Vercel):** $0/month = $0/year

**You save:** $192-420 per year! 💰

---

Good luck! Your new website will be live soon! 🚀
