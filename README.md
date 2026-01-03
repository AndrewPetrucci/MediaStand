# Media Stand

A lightweight, customizable mixed media dashboard that displays embedded content from multiple platforms in a single, stylish interface.

## Features

- 🎨 **Animated Gradient Background** - Smooth color transitions between purple, blue, and black
- 🎵 **Deezer Integration** - Display your favorite albums with embedded Deezer widgets
- 📺 **YouTube Integration** - Embed YouTube videos alongside music
- 📱 **Responsive Layout** - Horizontal scrolling media sections
- 🎯 **Easy Customization** - Simple HTML/CSS structure for quick modifications
- 🌙 **Dark Theme** - Beautiful dark panels with semi-transparent backgrounds

## Getting Started

### Prerequisites
- Any modern web browser
- A local web server (optional, for testing)

### Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/andrewpetrucci/MediaManiacStandAnarcyWebRing.git
   cd MediaManiacStandAnarcyWebRing
   ```

2. **Serve locally (optional):**
   ```bash
   python -m http.server 8000
   ```
   Then open `http://localhost:8000` in your browser.

3. **Or just open `index.html` directly in your browser**

## Customization

### Adding Deezer Albums

1. Find the album on Deezer
2. Copy the embed URL from the widget
3. Add an iframe to the "Deezer Delights" section:

```html
<iframe title="deezer-widget" src="https://widget.deezer.com/widget/dark/album/ALBUM_ID"
    frameborder="0" allowtransparency="true" 
    allow="encrypted-media; clipboard-write"></iframe>
```

### Adding YouTube Videos

1. Find the video on YouTube
2. Copy the embed code
3. Add an iframe to the "Youtube Yarn" section:

```html
<iframe width="560" height="315" 
    src="https://www.youtube.com/embed/VIDEO_ID" 
    title="YouTube video player" frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
```

### Styling

All colors and spacing are controlled by CSS variables in the `<style>` section:

- **Background Gradient**: Modify the `body` linear-gradient colors
- **Panel Colors**: Edit `.dark-panel` background and color values
- **Text Colors**: Adjust `h1`, `h2`, and text color properties
- **Spacing**: Modify `padding`, `margin`, and `gap` values

## Project Structure

```
MediaManiacStandAnarcyWebRing/
├── index.html          # Main HTML file
├── README.md           # This file
└── ...
```

## Browser Support

Works on all modern browsers that support:
- CSS Grid/Flexbox
- CSS Animations
- HTML5 Embedded Content

## License

Feel free to use and modify this project as needed!

## Tips

- Use the horizontal scroll to view more media items
- All iframes automatically resize with the page
- Dark panels are semi-transparent, allowing the gradient background to show through
- Add more sections by copying the `.dark-panel` div and changing the `<h2>` title

Enjoy your media mashup! 🎬🎵
