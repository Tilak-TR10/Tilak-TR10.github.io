# How to Add Your Profile Photo

## Quick Steps:

### 1. Prepare Your Photo
- Use a professional photo (headshot or casual professional photo)
- **Recommended size**: 400x400 pixels or larger (square works best)
- **Format**: JPG or PNG
- **File size**: Keep it under 500KB for fast loading

### 2. Name Your Photo File
- Rename your photo to: `profile.jpg` (or `profile.png`)
- Keep the name simple and lowercase

### 3. Add Photo to Your Website

**Option A: Same folder as HTML file (Easiest)**
1. Put your photo file (`profile.jpg`) in the **same folder** as `portfolio-final.html`
2. Done! The website will automatically find it

**File structure should look like:**
```
your-portfolio-folder/
├── portfolio-final.html
├── profile.jpg          ← Your photo here
└── README.md
```

**Option B: Create an images folder (Organized)**
1. Create a folder called `images` next to your HTML file
2. Put your photo in the `images` folder
3. Update the HTML (line 291) to:
   ```html
   <img src="images/profile.jpg" alt="Tilak Raval" class="profile-photo">
   ```

**File structure:**
```
your-portfolio-folder/
├── portfolio-final.html
├── images/
│   └── profile.jpg      ← Your photo here
└── README.md
```

### 4. Deploy to GitHub Pages

When deploying to GitHub:
1. Upload **both** `portfolio-final.html` AND `profile.jpg` to your repository
2. Make sure they're in the same folder (or use the images folder structure)
3. GitHub Pages will serve both files

---

## Tips for Best Results:

✅ **Do:**
- Use a square photo (1:1 ratio) - it looks best
- Keep background simple and professional
- Make sure your face is well-lit
- Use recent photo
- Keep file size under 500KB

❌ **Don't:**
- Use extremely large files (will slow down your site)
- Use low-resolution or blurry photos
- Use photos with distracting backgrounds

---

## Photo Styling Options:

The photo currently has:
- **Rounded corners** (12px border radius)
- **Border** (3px solid)
- **Subtle shadow**

### Want a circular photo instead?
Change line 165 in the HTML from:
```css
border-radius: 12px;
```
to:
```css
border-radius: 50%;
```

### Want no border?
Remove or comment out line 166:
```css
/* border: 3px solid var(--border); */
```

### Want a different size?
Change lines 162-163:
```css
width: 250px;    /* Make it bigger */
height: 250px;   /* Make it bigger */
```

---

## Testing Locally:

Before deploying, test that your photo loads:

1. **Simple method**: Just double-click `portfolio-final.html` and check if photo appears
2. **Better method**: Run a local server:
   ```bash
   # Navigate to your folder
   cd path/to/your/portfolio
   
   # Start server
   python -m http.server 8000
   
   # Open browser to: http://localhost:8000
   ```

---

## Troubleshooting:

### Photo not showing?
1. ✅ Check the file name matches exactly: `profile.jpg`
2. ✅ Check the photo is in the same folder as the HTML
3. ✅ Check the file extension (`.jpg` not `.jpeg`)
4. ✅ Try refreshing your browser (Ctrl+Shift+R or Cmd+Shift+R)

### Photo too big/small?
- Edit the CSS (lines 162-163) to adjust size

### Photo looks stretched?
- Use a square photo (same width and height)
- The `object-fit: cover` setting will handle the rest

---

## Image Optimization (Optional):

To make your photo load faster:

1. **Online tools** (free):
   - https://tinypng.com - Compress image
   - https://squoosh.app - Compress & resize
   - https://www.iloveimg.com - Resize & optimize

2. **Recommended settings**:
   - Width: 400-600px
   - Quality: 80-90%
   - Format: JPG (for photos)

---

**That's it!** Your professional photo will appear next to your name and bio, just like on academic websites! 📸✨
