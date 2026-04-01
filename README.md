# Web Harmonium 🎵

> **Play a real sampled Indian classical harmonium directly in your browser.** No plugins, no installation. Use your keyboard or MIDI device to learn ragas, explore Sargam notation, and add reverb effects. Built with Web Audio API.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-harmoniumweb.vercel.app-blue?style=flat-square)](https://harmoniumweb.vercel.app/)
[![GitHub Stars](https://img.shields.io/github/stars/devchauhann/harmoniumweb?style=flat-square)](https://github.com/devchauhann/harmoniumweb)
[![GitHub License](https://img.shields.io/github/license/devchauhann/harmoniumweb?style=flat-square)](LICENSE)
[![GitHub Issues](https://img.shields.io/github/issues/devchauhann/harmoniumweb?style=flat-square)](https://github.com/devchauhann/harmoniumweb/issues)

![Web Harmonium](og-image.png)

---

## ✨ Features

- 🎹 **Keyboard Playing** - Use your computer keyboard to play Indian classical ragas
- 🎛️ **MIDI Support** - Connect any MIDI device (keyboards, controllers) for authentic control
- 📝 **Sargam Notation** - Real-time Sargam notation logging as you play
- 🔊 **Reverb Effects** - Add realistic acoustic space and depth
- 🎼 **Multi-Octave** - Explore 7 different octaves
- 🎵 **Extra Reeds** - Layer harmonics (0-6 stacked notes)
- 📱 **Mobile Ready** - Fully responsive design with landscape support
- ⚡ **No Installation** - Pure browser-based, no plugins needed
- 🔒 **Secure** - HTTPS ready with security headers
- 📲 **PWA Ready** - Installable as a progressive web app

---

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/devchauhann/harmoniumweb.git
cd harmoniumweb

# 2. Open in browser (no build required!)
# Option A: Open index.html directly
open index.html

# Option B: Use a local server (recommended)
python3 -m http.server 8000
# Then visit http://localhost:8000
```

**Live Demo:** [harmoniumweb.vercel.app](https://harmoniumweb.vercel.app/)

---

## 🎮 How to Play

### Keyboard Mapping

**White Keys (Natural Notes):**
```
` q w e r t y u i o p [ ] \
```

**Black Keys (Sharp Notes):**
```
1 2 4 5 7 8 9 - =
```

### Notation Controls
- `Tab` - Add comma (rest) to notation
- `Backspace` - Delete last character
- `Delete` - Clear entire notation

### Controls Panel

| Control | Function | Range |
|---------|----------|-------|
| **Volume** | Adjust sound level | 0-100% |
| **Reverb** | Toggle acoustic effect | On/Off |
| **Transpose** | Change root note | -11 to +11 semitones |
| **Octave** | Select octave | 0-6 |
| **Extra Reeds** | Layer harmonics | 0-6 notes |
| **MIDI Device** | Connect MIDI hardware | Auto-detect |

---

## 🏗️ Project Structure

```
harmoniumweb/
├── index.html              # Main application (single file)
├── manifest.json           # PWA configuration
├── robots.txt              # SEO crawler directives
├── sitemap.xml             # Desktop sitemap
├── sitemap-mobile.xml      # Mobile sitemap
├── README.md               # This file
├── og-image.png            # Social media preview (1200x630)
├── harmonium.wav           # Harmonium audio sample
├── reverb.wav              # Reverb impulse response
├── .htaccess               # Server configuration
└── favicon/                # App icons (all formats)
    ├── favicon.ico
    ├── favicon.svg
    ├── favicon-16x16.png
    ├── favicon-32x32.png
    ├── favicon-96x96.png
    ├── apple-touch-icon.png
    ├── browserconfig.xml
    └── manifest.webmanifest
```

---

## 🔍 SEO & Discoverability

✅ **Comprehensive Meta Tags** - Title, description, keywords, author  
✅ **Open Graph Tags** - Optimized for social media sharing  
✅ **Twitter Card** - Special formatting for Twitter/X  
✅ **Schema Markup** - JSON-LD for Google Rich Snippets  
✅ **Sitemaps** - Desktop & mobile sitemaps for crawlers  
✅ **Favicon** - Multi-format icons for all platforms  
✅ **PWA Manifest** - Progressive Web App configuration  
✅ **Mobile Optimized** - Responsive design with media queries  
✅ **Performance** - Gzip compression, browser caching, HTTP/2  
✅ **Security** - HSTS, CSP, X-Frame-Options headers  

### Ranking Keywords
- "web harmonium"
- "online harmonium"
- "Indian classical music"
- "Sargam notation"
- "harmonium player"
- "MIDI harmonium"
- "music education"

---

## 🌐 Browser Support

| Browser | Min Version | Status |
|---------|------------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |
| Mobile Safari | 14+ | ✅ Landscape Mode |
| Chrome Mobile | 90+ | ✅ Landscape Mode |

---

## 💻 Tech Stack

- **Frontend** - HTML5, CSS3 (variables, media queries, animations)
- **Audio** - Web Audio API, MIDI API, Sampled harmonium sounds
- **State** - localStorage for persistence
- **PWA** - Service Worker, Manifest, Installable
- **Performance** - Gzip, browser caching, resource preconnection
- **Deployment** - Vercel (free tier)

---

## 🎓 Learning Resources

### Understanding Indian Classical Music
- [Sargam Notation Guide](https://en.wikipedia.org/wiki/Sargam)
- [Raga Basics](https://en.wikipedia.org/wiki/Raga)
- [Harmonium in Indian Music](https://en.wikipedia.org/wiki/Harmonium)

### Web Audio API
- [MDN Web Audio API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [Web Audio API Specification](https://www.w3.org/TR/webaudio/)

### MIDI API
- [Web MIDI API Docs](https://developer.mozilla.org/en-US/docs/Web/API/Web_MIDI_API)

---

## 📊 Performance Metrics

- **Load Time** - < 1 second (optimized assets)
- **FCP** - First Contentful Paint < 800ms
- **LCP** - Largest Contentful Paint < 1.2s
- **CLS** - Cumulative Layout Shift < 0.1
- **Performance Score** - 95+/100 (Lighthouse)

---

## 🛠️ Development

### Building Locally

```bash
# No build step required! Just serve the files
python3 -m http.server 8000

# Or with Node.js
npx http-server

# Or with Live Server (VS Code extension)
# Install: "Live Server" by Ritwick Dey
# Right-click index.html > Open with Live Server
```

### Customization

The entire app is in a single `index.html` file for simplicity:
- CSS variables are at the top for easy theming
- Audio parameters are easily adjustable
- Keyboard mapping can be modified
- Add your own effects or samples

---

## 🤝 Contributing

Contributions are welcome! Here's how:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Make** your changes
4. **Test** in multiple browsers
5. **Commit** with clear messages (`git commit -m 'Add amazing feature'`)
6. **Push** to your branch (`git push origin feature/amazing-feature`)
7. **Open** a Pull Request

### Issues & Suggestions
- Found a bug? [Report it](https://github.com/devchauhann/harmoniumweb/issues/new)
- Have an idea? [Suggest it](https://github.com/devchauhann/harmoniumweb/discussions)

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Dev Chauhan**
- GitHub: [@devchauhann](https://github.com/devchauhann)
- Twitter: [@devchauhann](https://twitter.com/devchauhann3)

---

## 🌟 Support

If you find this project useful:
- ⭐ Star the repository
- 🐛 Report bugs
- 💡 Suggest features
- 🔄 Share with friends
- 📢 Follow on social media

---

## 📈 Stats & Analytics

[![GitHub followers](https://img.shields.io/github/followers/devchauhann?style=social)](https://github.com/devchauhann)
[![Twitter followers](https://img.shields.io/twitter/follow/devchauhann?style=social)](https://twitter.com/devchauhann)

---

## 🎵 Special Thanks

- [Web Audio API Community](https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API)
- [MIDI Specification](https://www.midi.org/)
- [Indian Classical Music Community](https://en.wikipedia.org/wiki/Indian_classical_music)

---

**Last Updated:** April 1, 2026  
**Current Version:** 1.0.0  
**Status:** ✅ Production Ready
