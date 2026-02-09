# File Organization Guide

## Required Folder Structure

```
valentine-website/
│
├── index.html                 (Main website file)
├── README.md                  (Instructions - you're reading this!)
│
├── images/                    (Your photos go here)
│   ├── memory1.jpg
│   ├── memory2.jpg
│   ├── memory3.jpg
│   ├── memory4.jpg
│   ├── memory5.jpg
│   └── memory6.jpg
│
├── gifs/                      (Your animated GIFs)
│   ├── left.gif              (Left side GIF)
│   └── right.gif             (Right side GIF)
│
└── music/                     (Your background music)
    └── romantic-song.mp3     (Background music file)
```

## Quick Customization Checklist

### ✅ Before Uploading to GitHub:

1. **Add Your Photos**
   - [ ] Replace 6 dummy images with your actual photos
   - [ ] Name them memory1.jpg through memory6.jpg
   - [ ] Place them in the `images/` folder

2. **Add Your GIFs**
   - [ ] Find 2 romantic/cute GIFs
   - [ ] Save as left.gif and right.gif
   - [ ] Place them in the `gifs/` folder
   - [ ] OR use online GIF URLs (Giphy, Tenor)

3. **Add Your Music**
   - [ ] Choose a romantic song (MP3 format)
   - [ ] Name it romantic-song.mp3
   - [ ] Place it in the `music/` folder

4. **Customize Text**
   - [ ] Edit photo captions in CONFIG.galleryImages
   - [ ] (Optional) Change the main question text
   - [ ] (Optional) Customize button messages

### 📝 Where to Edit in index.html:

**Line ~529-570: CONFIG Section**
```javascript
const CONFIG = {
    leftGif: 'gifs/left.gif',      // ← Change GIF paths here
    rightGif: 'gifs/right.gif',
    musicPath: 'music/romantic-song.mp3',  // ← Change music path here
    
    galleryImages: [
        {
            src: 'images/memory1.jpg',    // ← Your image path
            title: 'Our First Date',       // ← Change title
            text: 'Custom description...'  // ← Change description
        },
        // ... repeat for all 6 images
    ]
};
```

### 🎨 Optional Customizations:

**Change Pink Color Scheme (Line ~21-27):**
```css
:root {
    --pink-bg: #FFE5EC;      /* Background color */
    --pink-accent: #FF69B4;  /* Accent color */
    --pink-dark: #FF1493;    /* Button color */
}
```

**Change Fonts (Line 11):**
Current fonts: Pacifico (headings) + Quicksand (body)
Replace the Google Fonts URL to use different fonts

**Change Main Question (Line ~370):**
```html
<h1>Will You Be My Valentine? 💝</h1>
```

### 🚀 Deployment Steps:

1. Create all folders (images, gifs, music)
2. Add your custom files
3. Test locally by opening index.html in a browser
4. Upload everything to GitHub
5. Enable GitHub Pages in repository settings
6. Share the link with your girlfriend!

### 💡 Pro Tips:

- **Image Dimensions**: 400x300 pixels works great
- **GIF Size**: Keep under 5MB for faster loading
- **Music Format**: MP3 is most compatible
- **Test Mobile**: Check how it looks on your phone
- **Privacy**: Make repository private if you don't want others to see

---

## Alternative: Using Online URLs (No File Upload)

If you prefer not to upload files, you can use online URLs:

**For GIFs:** Use Giphy.com or Tenor.com
```javascript
leftGif: 'https://media.giphy.com/media/YOUR-GIF-ID/giphy.gif'
```

**For Images:** Upload to Imgur.com or use Unsplash
```javascript
src: 'https://i.imgur.com/YOUR-IMAGE.jpg'
```

**For Music:** Host on SoundCloud or use a file hosting service
```javascript
musicPath: 'https://your-hosting-service.com/song.mp3'
```

---

Need help? Check README.md for full instructions!
