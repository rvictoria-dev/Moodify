# Moodify

### ₊⊹ About

Moodify is a minimalist web app inspired by Spotify's interface. The project lets you showcase memorable excerpts from song lyrics and your favorite tracks in elegant, clean, and highly shareable cards. The project is also very helpful for learning about semantic tags and how to use Flexbox.

<img width="1149" height="620" alt="image" src="https://github.com/user-attachments/assets/81809929-b62b-49e1-b431-062c80f395bb" />

---

### ★ Features

- **Full-Screen Centering:** Combined use of `min-height: 100vh` with `display: flex`, `align-items: center`, and `justify-content: center` on the `body` element to keep the card perfectly centered on the screen.

- **Controlled Vertical Flow:** Configuring the main container with `flex-direction: column` to neatly stack the header, song lyrics, and footer.

- **Directional Alignment:** Use of Flexbox in the inner blocks (.track-header, .mood-text, and .track-footer) to precisely manage the behavior and alignment axes of icons, text, and images.

- **Visual Fidelity:** Faithful reproduction of the Spotify player’s visual identity, using rounded corners (border-radius) and balanced size proportions.

- **Optimized Typography:** Integration with Google Fonts to load specific weight variations of the Inter font (600, 700, and 800), allowing for the creation of a clear visual hierarchy between the song title and the lyrics.

---

### ⚙️ Tech Stack

- **HTML5**
- **CSS3**
- **Google Fonts (Inter):** External integration of the *Inter* font, optimized for selective loading of heavy font weights (`600`, `700`, `800`), ensuring the distinctive, bold look characteristic of Spotify’s typography.

---

### 🖿 Project structure

```
moodify/
├── Assets/
│   ├── album-cover.png
│   └── spotify-icon.svg
├── index.html
├── style.css
└── README.md
```

---

### .ᐟ.ᐟ How It Works

1. **Three-Dimensional Alignment of the `body`**
The browser interprets the `body` as a large, flexible screen. By setting `min-height: 100vh`, we ensure that it occupies the entire visible height of the screen. The properties `align-items: center` (vertical axis) and `justify-content: center` (horizontal axis) work together to position the card exactly in the center of the screen.

2. **The Stacking Flow of the Card (`.mood-card`)**
The main card operates under the concept of **column direction** (`flex-direction: column`). This changes the natural behavior of the blocks: instead of appearing side by side, the `<header>`, the text of the letter (`.mood-text`), and the `<footer>` are automatically stacked vertically in an organized manner.

3. **Internal Layout of the Blocks**
Each row of the card manages its own elements independently:
* **Header (`.track-header`):** Aligns the album cover and text horizontally using Flexbox. The right margin is strategically controlled with `margin-right` to provide optimal spacing relative to the right edge.
* **Lyrics (`.mood-text`):** Set to a comfortable line height (`line-height: 1.5`) to stack the song lyrics and create a central block with bold, robust typography.
* **Footer (`.track-footer`):** Uses the `display: flex` property with `gap: 2px` to precisely position the Spotify icon next to the brand text, maintaining a visual identity identical to that of the original app.
