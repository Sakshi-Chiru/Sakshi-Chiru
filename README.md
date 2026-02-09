# Valentine's Day Website 💝

A beautiful, interactive Valentine's Day website with adaptive design that works perfectly on both phones and laptops.

## Features ✨

- **Interactive Question Page**: 
  - Glass-morphism design with pink theme
  - Animated GIFs on the sides
  - Playful "No" button that bounces and moves away from cursor
  - Background music that plays after first interaction
  - Custom messages in Hindi/English mix
  - Confetti celebration when "Yes" is clicked

- **Photo Gallery Page**:
  - Responsive grid layout
  - Smooth animations
  - Custom captions for each memory
  - Glass-morphism cards with hover effects

- **Fully Responsive**: Works beautifully on mobile phones, tablets, and desktop computers

## Setup Instructions 🚀

### 1. Download the Files

Save the `index.html` file to your computer.

### 2. Create Folder Structure

Create the following folder structure:

```
valentine-website/
├── index.html
├── images/
│   ├── memory1.jpg
│   ├── memory2.jpg
│   ├── memory3.jpg
│   ├── memory4.jpg
│   ├── memory5.jpg
│   └── memory6.jpg
├── gifs/
│   ├── left.gif
│   └── right.gif
└── music/
    └── romantic-song.mp3
```

### 3. Add Your Custom Content

#### Adding Your Photos:
1. Place 6 photos in the `images/` folder
2. Name them: `memory1.jpg`, `memory2.jpg`, etc.
3. Edit the `CONFIG.galleryImages` array in the HTML file (around line 537):

```javascript
galleryImages: [
    {
        src: 'images/memory1.jpg',
        title: 'Your Custom Title',
        text: 'Your custom description here...'
    },
    // ... add all 6 images
]
```

#### Adding Your GIFs:
1. Place your GIFs in the `gifs/` folder
2. Update the CONFIG section (around line 529):

```javascript
leftGif: 'gifs/left.gif',
rightGif: 'gifs/right.gif',
```

#### Adding Background Music:
1. Place your music file (MP3 format) in the `music/` folder
2. Name it `romantic-song.mp3` OR update the CONFIG:

```javascript
musicPath: 'music/your-song-name.mp3',
```

### 4. Deploy to GitHub Pages

#### Step 1: Create a GitHub Repository
1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon → "New repository"
3. Name it: `valentine-website` (or any name you like)
4. Make it **Public**
5. Click "Create repository"

#### Step 2: Upload Your Files
1. Click "uploading an existing file"
2. Drag and drop ALL your files:
   - `index.html`
   - The `images/` folder
   - The `gifs/` folder
   - The `music/` folder
3. Click "Commit changes"

#### Step 3: Enable GitHub Pages
1. Go to your repository Settings
2. Scroll down to "Pages" section (left sidebar)
3. Under "Source", select "main" branch
4. Click "Save"
5. Wait 1-2 minutes, then visit: `https://YOUR-USERNAME.github.io/valentine-website/`

## Customization Options 🎨

### Change Colors:
Edit the CSS variables at the top of the `<style>` section:

```css
:root {
    --pink-bg: #FFE5EC;        /* Main background */
    --pink-light: #FFF0F5;     /* Light pink */
    --pink-accent: #FF69B4;    /* Accent pink */
    --pink-dark: #FF1493;      /* Dark pink */
}
```

### Change Messages:
All messages are in the JavaScript section. Search for these texts and replace:
- "Will You Be My Valentine?"
- "Why didn't you report the bug..."
- "Himmat hai toh firse No bolke dikhao"
- "Congratulations, mujhe toh pata hi tha..."

### Add More Photos:
To add more than 6 photos, add more objects to the `CONFIG.galleryImages` array:

```javascript
{
    src: 'images/memory7.jpg',
    title: 'New Memory',
    text: 'Description here'
}
```

## Troubleshooting 🔧

**Music doesn't play?**
- Most browsers block autoplay. The music plays after the first "No" button click
- Make sure your music file is in MP3 format
- Check the file path in CONFIG

**Images don't show?**
- Check that file names match exactly (case-sensitive)
- Verify all images are in the `images/` folder
- Use JPG, JPEG, or PNG formats

**GIFs don't show?**
- Verify GIF file paths in CONFIG
- Make sure GIFs are in the `gifs/` folder
- You can also use online GIF URLs (like Giphy)

## Browser Compatibility 🌐

Works on:
- ✅ Chrome/Edge (recommended)
- ✅ Safari
- ✅ Firefox
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Tips 💡

1. **Image Size**: Keep images under 2MB each for faster loading
2. **Music Length**: Use a 2-3 minute song that loops nicely
3. **Test First**: Open `index.html` locally in your browser before deploying
4. **Mobile First**: Always test on your phone after deploying

## License

Free to use and customize for personal purposes. Made with ❤️

---

**Need help?** If something doesn't work, double-check:
1. File names match exactly
2. Folder structure is correct
3. All files are uploaded to GitHub
4. GitHub Pages is enabled in settings

Enjoy your special Valentine's website! 💕
