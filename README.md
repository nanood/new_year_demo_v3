# 🎄 Interactive 3D Christmas Tree

An interactive 3D Christmas tree web application with gesture control, music visualization, and photo integration. Built with Three.js and MediaPipe Hands.

[**🎮 Live Demo**](https://mrfeixiang.github.io/christmas-tree-3d/) | [**📖 Documentation**](./docs/)

![Christmas Tree Demo](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Three.js](https://img.shields.io/badge/Three.js-r128-green.svg)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Hands-orange.svg)

<p align="center">
  <img src="screenshot.png" alt="Christmas Tree Screenshot" width="800">
</p>

## ✨ Features

### 🤚 Gesture Control
Control the 3D scene with hand gestures using your webcam:
- **✊ Fist** - Form particles into a Christmas tree
- **✋ Open Palm** - Disperse particles and rotate scene
- **🤏 Pinch** - Focus on a single photo
- **✌️ Victory** - Gallery mode (show all photos)
- **🤲 Two Hands** - Pinch zoom photos
- **👍👍 Double Thumbs Up** - Trigger fireworks effect

### 🎵 Music Integration
- Upload MP3 files
- Paste Suno AI or audio URLs
- Real-time audio visualization
- Particles dance to the music
- Dynamic lighting effects
- Volume control

### 📷 Photo Management
- Upload multiple photos
- Single photo focus mode
- Gallery grid view
- Two-hand pinch to zoom (50% - 300%)
- Smooth transitions

### 🎨 Visual Effects
- 2000+ particle system
- Golden ornaments and snowflakes
- Dynamic lighting (spotlights & point lights)
- Music-reactive particles and lights
- Smooth animations

### ⌨️ Keyboard Shortcuts
- **H** - Hide/show UI
- **M** or **Space** - Play/pause music

## 🚀 Quick Start

### Option 1: Direct Use (No Installation)
1. Download `christmas-tree-3d.html`
2. Open in a modern browser (Chrome/Safari recommended)
3. Allow camera access when prompted
4. Make gestures to interact!

### Option 2: GitHub Pages
Visit the live demo: [https://mrfeixiang.github.io/christmas-tree-3d/](https://mrfeixiang.github.io/christmas-tree-3d/)

### Option 3: Local Development
```bash
# Clone the repository
git clone https://github.com/mrfeixiang/christmas-tree-3d.git

# Navigate to directory
cd christmas-tree-3d

# Open with a local server (required for some features)
# Using Python 3:
python -m http.server 8000

# Or using Node.js:
npx http-server

# Open browser to http://localhost:8000
```

## 📖 How to Use

### 1. Upload Music
Click **"🎼 更换音乐"** button and choose:
- **Upload MP3** - Select from your computer
- **Paste URL** - Use Suno AI or any audio URL
- **Example Music** - Try the demo music

### 2. Upload Photos
Click **"📷 上传照片"** to add your photos from iCloud or local storage

### 3. Make Gestures
Position your hands in front of the webcam and make gestures to control:
- Form the Christmas tree
- Disperse particles
- View photos
- Zoom photos with two hands
- Trigger fireworks

## 🎮 Gesture Guide

<table>
<tr>
<td align="center">
<img src="docs/gestures/fist.png" width="80"><br>
<b>Fist</b><br>
Form Tree
</td>
<td align="center">
<img src="docs/gestures/palm.png" width="80"><br>
<b>Open Palm</b><br>
Disperse
</td>
<td align="center">
<img src="docs/gestures/pinch.png" width="80"><br>
<b>Pinch</b><br>
Focus Photo
</td>
<td align="center">
<img src="docs/gestures/victory.png" width="80"><br>
<b>Victory</b><br>
Gallery
</td>
</tr>
<tr>
<td align="center">
<img src="docs/gestures/two-hands.png" width="80"><br>
<b>Two Hands</b><br>
Zoom Photo
</td>
<td align="center">
<img src="docs/gestures/thumbs-up.png" width="80"><br>
<b>Double Thumbs</b><br>
Fireworks
</td>
</tr>
</table>

## 🛠️ Technical Stack

- **Three.js (r128)** - 3D rendering
- **MediaPipe Hands** - Hand tracking and gesture recognition
- **Web Audio API** - Music visualization
- **Canvas API** - Hand skeleton drawing
- **WebRTC** - Webcam access
- **Vanilla JavaScript** - No frameworks required

## 📦 Project Structure

```
christmas-tree-3d/
├── christmas-tree-3d.html    # Main application (single file!)
├── README.md                  # This file
├── docs/                      # Documentation
│   ├── MUSIC-SETUP-GUIDE.md
│   ├── SUNO-MUSIC-GUIDE.md
│   ├── MUSIC-QUICK-START.md
│   └── MUSIC-FIX-QUICK-REF.md
├── audio-test.html            # Audio debugging tool
└── LICENSE                    # MIT License
```

## 🎵 Adding Music

### Method 1: Upload MP3 (Recommended)
1. Click "🎼 更换音乐"
2. Click "选择文件" or drag-drop MP3
3. Music plays automatically

### Method 2: Use Suno AI
1. Go to [suno.com](https://suno.com)
2. Generate Christmas music with AI
3. Copy the audio URL
4. Paste in the app
5. Click "加载音乐"

**Suno Prompt Examples:**
```
"Upbeat Christmas music with bells, piano and strings, festive and joyful"
"Peaceful Christmas ambient music with soft piano and gentle chimes"
"Rock Christmas song with electric guitar and drums, energetic"
```

### Method 3: Use Audio URLs
Paste any direct audio URL from:
- Pixabay Music
- Mixkit
- Your own server
- Google Drive/Dropbox direct links

See [SUNO-MUSIC-GUIDE.md](./docs/SUNO-MUSIC-GUIDE.md) for detailed instructions.

## 🖼️ Browser Compatibility

| Browser | Version | Status |
|---------|---------|--------|
| Chrome | 90+ | ✅ Fully Supported |
| Safari | 14+ | ✅ Fully Supported |
| Firefox | 88+ | ✅ Fully Supported |
| Edge | 90+ | ✅ Fully Supported |

**Requirements:**
- WebGL support
- Webcam access
- Modern JavaScript (ES6+)

## 📱 Platform Support

- ✅ **Desktop** - iMac, Windows PC, Linux
- ✅ **Laptop** - MacBook, Windows Laptop
- ⚠️ **Tablet** - Limited (gesture control may be difficult)
- ❌ **Mobile** - Not recommended (small screen, no reliable hand tracking)

## 🎯 Performance Tips

- **Particle Count**: Reduce from 2000 to 1000 for slower machines
- **Music File**: Use MP3 < 5MB
- **Browser**: Chrome recommended for best performance
- **Lighting**: Close other browser tabs

## 🐛 Troubleshooting

### No Camera Access?
- Check browser permissions (Settings > Camera)
- Try Chrome if Safari has issues
- Ensure no other app is using the camera

### Gestures Not Detecting?
- Ensure good lighting
- Keep hands centered in webcam view
- Adjust `minDetectionConfidence` in code (line 478)

### No Music?
- Click the play button (autoplay is blocked by browsers)
- Use the audio test tool: `audio-test.html`
- Try uploading a local MP3 file
- See [MUSIC-FIX-QUICK-REF.md](./docs/MUSIC-FIX-QUICK-REF.md)

### Performance Issues?
- Reduce particle count (line 45: change 2000 to 1000)
- Lower video resolution (line 463)
- Close other applications

## 🎓 Learning Resources

This project is great for learning:
- **Three.js Basics** - Scene, Camera, Renderer
- **Particle Systems** - BufferGeometry, Points
- **Web Audio API** - Audio visualization
- **MediaPipe** - Hand tracking and gesture recognition
- **JavaScript ES6+** - Modern JavaScript features

### Code Structure
The code is organized into sections:
1. Configuration and Constants
2. Three.js Scene Setup
3. Particle System
4. Fireworks Effect
5. Photo Management
6. MediaPipe Gesture Recognition
7. Music Control
8. Animation Loop

Each section has detailed comments for learning.

## 🤝 Contributing

Contributions are welcome! Here are some ideas:
- Add more gestures (thumbs up, peace sign)
- Implement bloom post-processing
- Add more particle types (gifts, ornaments)
- Create preset Christmas tree styles
- Add AR mode for mobile
- Multi-language support

### How to Contribute
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Three.js** - 3D graphics library
- **MediaPipe** - Google's ML solutions
- **Pixabay** - Free music resources
- **Suno AI** - AI music generation
- **Claude** - AI assistant by Anthropic

## 📧 Contact

Your Name - [@yourtwitter](https://twitter.com/yourtwitter)

Project Link: [https://github.com/mrfeixiang/christmas-tree-3d](https://github.com/mrfeixiang/christmas-tree-3d)

## 🌟 Show Your Support

Give a ⭐️ if this project helped you!

---

<p align="center">
Made with ❤️ for Christmas 🎄
</p>

<p align="center">
<a href="#top">Back to Top</a>
</p>
