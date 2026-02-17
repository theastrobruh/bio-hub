# Bio Link Hub Template 🌌

A modern, tech-themed personal hub website (Bio Link) designed to showcase your profile, social links, and creative work.

**Features:**
*   **Starfield Background**: Animated canvas background with stars and shooting stars.
*   **Neon/Tech Aesthetic**: 'Orbitron' typography and glowing neon effects.
*   **Interactive Profile**: Hover effects for profile pictures (Static -> Animated).
*   **Mini Music Player**: Floating widget to play background music via YouTube.
*   **Responsive**: Fully optimized for mobile and desktop.
*   **No Frameworks**: Pure HTML, CSS, and JS. Lightweight and fast.

---

## 🚀 Getting Started

1.  **Clone or Download** this repository.
2.  Open `index.html` in your browser to see the live site.
3.  Deploy to **GitHub Pages** (Settings > Pages) to share it with the world.

---

## 🛠️ Customization Guide

All configuration happens directly in the `index.html` file. Look for the `app` object inside the `<script>` tag at the bottom of the file.

### 1. Profile Information
Change your name, bio, and footer text.

```javascript
defaultData: {
    nombre: "Your Name",
    bio: "Your Short Bio Here",
    footer: "© 2026 - Your Brand"
    // ...
}
```

### 2. Profile Photo (Static & Animated)
You can use a simulated "Live Photo" effect. Place your images in `assets/images/`.

*   **photoStatic**: The image shown by default.
*   **photoAnimated**: A GIF or WEBP that plays when hovering (desktop) or tapping (mobile).

```javascript
// Local Photo Configuration
photoStatic: "./assets/images/avatar.jpg", 
photoAnimated: "./assets/images/avatar-animated.gif", 
```
> **Tip:** If you don't have an animated version, set both paths to the same static image.

### 3. Links
Add your social media links to the `enlaces` array. You can customize the `titulo` (Title), `url`, `icono` (Icon), and `color` (Hover/Border Color).

```javascript
enlaces: [
    { 
        titulo: "Instagram", 
        url: "https://instagram.com/user", 
        icono: "📸", 
        color: "#ff0069" // Custom color for this button
    },
    // Add more...
]
```

### 4. Music Player 🎵
The mini player uses a YouTube video ID to play audio in the background.

1.  Find a video on music.youtube.com or youtube.com.
2.  Copy the **Video ID** from the URL (e.g., `v=j4Wq42Hyxxo` -> `j4Wq42Hyxxo`).
3.  Paste it into the config:

```javascript
musicVideoId: "j4Wq42Hyxxo", // Change this ID
```

---

## 📂 File Structure

```
/
├── index.html        # Main file (Code & Config)
├── README.md         # Documentation
└── assets/
    └── images/       # Store your local photos/GIFs here
```

## 📜 License
Free to use and modify for your personal usage.
