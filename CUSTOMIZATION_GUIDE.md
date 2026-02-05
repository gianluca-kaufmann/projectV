# Valentine's Website Customization Guide

## How to Edit Text & Design Yourself

### 1. FIRST PAGE (Landing Page)

Open `index.html` and find this section (around line 270):

```html
<div id="initial-screen" class="initial-screen">
    <h1>February 14th</h1>
    <p class="subtitle">Something awaits you</p>
    <button class="reveal-button" onclick="revealSurprise()">Open</button>
</div>
```

**To customize:**
- Change `February 14th` to any title you want
- Change `Something awaits you` to any subtitle
- Change `Open` to any button text (e.g., "Click Here", "For You", etc.)

**To change colors:**
Find these lines near the top (around line 45-60):
- `background: linear-gradient(135deg, #f5f3f0 0%, #e8e4df 100%);` - Page background
- `color: #3a3a3a;` - Main text color (dark gray)
- `color: #6a6a6a;` - Subtitle color (medium gray)
- `background: #3a3a3a;` - Button color

### 2. SECOND PAGE (Gallery & Message)

#### Change the Love Message

Find this section (around line 319):

```html
<div class="love-message">
    <h2>Happy Valentine's Day</h2>
    <p>Every moment with you is a treasure.</p>
    <p>Thank you for filling my life with love and laughter.</p>
    <p>Here's to many more beautiful memories together.</p>
    <div class="signature">Forever yours ♥</div>
</div>
```

**To customize:**
- Change the heading `Happy Valentine's Day`
- Add or remove `<p>` lines for different messages
- Change the signature `Forever yours ♥`

#### Add More Flower Emojis

Find the floating emojis section (around line 308) and add more:

```html
<div class="floating-emoji" style="top: 50%; left: 20%; animation-delay: 1s;">🌻</div>
```

Change:
- `top: 50%` - vertical position (0% = top, 100% = bottom)
- `left: 20%` - horizontal position (0% = left, 100% = right)
- `animation-delay: 1s` - when it starts floating
- The emoji itself (🌸 🌺 🌷 🌹 💐 🌼 🌻 💕 ❤️ 💖)

### 3. CHANGING PHOTOS

Replace any of these image files with your own (keep the same filename):
- `IMG_1332.jpeg`
- `IMG_4733.jpeg`
- `IMG_7259.jpeg`
- `IMG_8906.jpeg`
- `IMG_9430.jpeg`
- `flowers.jpg` (the center image)

Or change the filenames in the HTML (around line 278-306):

```html
<img src="YOUR_PHOTO.jpg" alt="Us">
```

### 4. CHANGING FONTS

Find the font declarations at the top (around line 12 and elsewhere):

```css
font-family: 'Garamond', 'Georgia', serif;
```

Popular alternatives:
- `'Times New Roman', serif` - Classic
- `'Helvetica', 'Arial', sans-serif` - Modern
- `'Courier New', monospace` - Typewriter style

### 5. CHANGING ANIMATIONS

#### Speed up/slow down animations
Find animation declarations and change the duration:
- `animation: fadeIn 1.5s ease;` → Change `1.5s` to `1s` (faster) or `2s` (slower)

#### Remove animations
Find the element and remove the entire `animation:` line.

### 6. QUICK COLOR SCHEME CHANGES

Search and replace these colors throughout the file:

**Current scheme (elegant neutral):**
- `#3a3a3a` - Dark gray text
- `#6a6a6a` - Medium gray text
- `#f5f3f0` - Light beige background
- `#e8e4df` - Slightly darker beige

**Romantic pink scheme:**
- Replace `#3a3a3a` with `#8b2653` (deep pink)
- Replace `#6a6a6a` with `#c2185b` (medium pink)
- Replace `#f5f3f0` with `#ffeef8` (light pink)
- Replace `#e8e4df` with `#ffd4e8` (pink tint)

**Blue romantic scheme:**
- Replace `#3a3a3a` with `#1a3a52` (deep blue)
- Replace `#6a6a6a` with `#4a6c8a` (medium blue)
- Replace `#f5f3f0` with `#e8f4f8` (light blue)
- Replace `#e8e4df` with `#d4e8f0` (blue tint)

### 7. TESTING YOUR CHANGES

1. Save the `index.html` file
2. Double-click `index.html` to open in your browser
3. Refresh the page (Cmd+R on Mac, Ctrl+R on Windows) to see changes
4. If something breaks, press Cmd+Z (Undo) to revert

---

## Pro Tips

- Make small changes and test frequently
- Keep a backup copy before major changes
- Use Find & Replace (Cmd+F or Ctrl+F) for changing colors throughout
- Comments in the code start with `<!--` and end with `-->` - you can add your own notes
