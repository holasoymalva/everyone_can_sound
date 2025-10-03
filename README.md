# 🎵 Everyone Can Sound

> **Transforming Visual Motion into Musical Art** - A revolutionary real-time ASCII art generator with AI-powered motion-to-music synthesis

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen)](https://holasoymalva.github.io/everyone_can_sound)
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Made with ❤️](https://img.shields.io/badge/Made%20with-❤️-red.svg)](https://github.com/holasoymalva)

## 🚀 What is Everyone Can Sound?

**Everyone Can Sound** is a cutting-edge web application that bridges the gap between visual art and music. Using advanced computer vision and audio synthesis, it transforms your camera feed into beautiful ASCII art while generating harmonious music based on your movements in real-time.

### ✨ Key Features

- 🎨 **Real-time ASCII Art Generation** - Convert your camera feed into stunning ASCII art
- 🎵 **Motion-to-Music Synthesis** - Generate beautiful pentatonic melodies based on your movements
- 🤖 **AI-Powered Background Removal** - Clean, professional-looking output with MediaPipe integration
- 📹 **Video Recording** - Capture and save your ASCII art sessions
- ⚡ **Zero Installation** - Runs entirely in your browser
- 🎛️ **Customizable Parameters** - Adjust resolution, sensitivity, and audio settings

## 🎯 Use Cases

- **Digital Art Creation** - Create unique ASCII art pieces
- **Music Therapy** - Generate calming music through gentle movements
- **Interactive Installations** - Perfect for museums, galleries, and exhibitions
- **Educational Tools** - Teach concepts of computer vision and audio synthesis
- **Entertainment** - Fun way to create art and music simultaneously
- **Accessibility** - Visual-to-audio conversion for enhanced experiences

## 🛠️ Technology Stack

- **Frontend**: React 18 with Babel (no build process required)
- **Computer Vision**: MediaPipe Selfie Segmentation
- **Audio Synthesis**: Web Audio API with custom oscillators
- **Motion Detection**: Custom pixel-difference algorithms
- **UI Components**: Lucide React icons
- **Styling**: Pure CSS with modern design principles

## 🚀 Quick Start

### Option 1: Direct Usage (Recommended)

1. **Clone the repository**
   ```bash
   git clone https://github.com/holasoymalva/everyone_can_sound.git
   cd everyone_can_sound
   ```

2. **Serve the files**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in browser**
   Navigate to `http://localhost:8000`

### Option 2: Live Demo

Visit the live demo at: [https://holasoymalva.github.io/everyone_can_sound](https://holasoymalva.github.io/everyone_can_sound)

## 📖 How to Use

### Basic Usage

1. **Grant Camera Permission** - Allow browser access to your camera
2. **Click "Start Camera"** - Begin the ASCII art generation
3. **Move Around** - Your movements will be converted to ASCII art
4. **Enable Music** - Toggle "Generate Music from Motion" for audio synthesis
5. **Adjust Settings** - Use sliders to customize resolution and sensitivity

### Advanced Features

#### 🎵 Music Generation
- **Enable Motion-to-Music**: Check the "Generate Music from Motion" box
- **Movement Mapping**: Different screen positions trigger different musical notes
- **Intensity Control**: Faster movements create louder, more complex harmonies
- **Pentatonic Scale**: Uses a pleasing 5-note scale for natural-sounding melodies

#### 🖼️ Background Removal
- **AI Segmentation**: Toggle "Remove Background" for clean, professional output
- **Real-time Processing**: Uses MediaPipe for instant background removal
- **Enhanced Focus**: Isolates subject for better ASCII art generation

#### 📹 Recording
- **Start Recording**: Click the record button to capture your session
- **Automatic Download**: Recordings are automatically saved as video files
- **High Quality**: Maintains resolution and frame rate during recording

## ⚙️ Configuration Options

### Resolution Settings
- **Low (20)**: Fast performance, chunky ASCII art
- **Medium (40)**: Balanced performance and detail
- **High (60)**: Detailed ASCII art, requires more processing power

### Motion Sensitivity
- **Low**: Only detects significant movements
- **Medium**: Balanced sensitivity (recommended)
- **High**: Detects subtle movements and gestures

### Audio Settings
- **Volume Control**: Automatic volume adjustment based on motion intensity
- **Note Duration**: 600ms per note for natural musical phrasing
- **Harmony**: Multiple simultaneous notes for rich musical textures

## 🎨 ASCII Art Characters

The application uses a carefully selected character set for optimal visual representation:

```
@%#*+=-:. 
```

- `@` - Darkest areas
- `%#*` - Dark to medium areas
- `+=-:` - Medium to light areas
- `.` - Light areas
- ` ` (space) - Brightest/transparent areas

## 🔧 Technical Details

### Motion Detection Algorithm

```javascript
// Simplified motion detection process
1. Capture current frame from camera
2. Compare with previous frame pixel by pixel
3. Calculate motion intensity in grid sections
4. Filter areas above motion threshold
5. Map motion areas to musical notes
6. Generate ASCII characters based on brightness
```

### Music Generation Process

```javascript
// Pentatonic scale frequencies (C major pentatonic)
const PENTATONIC_SCALE = [261.63, 293.66, 329.63, 392.00, 440.00];

// Motion-to-music mapping
- X-axis position → Note selection
- Y-axis position → Octave variation
- Motion intensity → Volume and harmony
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Development Setup

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Make your changes**
4. **Test thoroughly**
5. **Submit a pull request**

### Contribution Ideas

- 🎵 **New Musical Scales** - Add different musical modes and scales
- 🎨 **ASCII Art Styles** - Implement different character sets and styles
- 🤖 **AI Enhancements** - Improve motion detection algorithms
- 📱 **Mobile Optimization** - Enhance mobile device performance
- 🎛️ **UI Improvements** - Design better control interfaces
- 🔊 **Audio Effects** - Add reverb, delay, and other audio processing

## 📊 Performance Optimization

### Browser Compatibility
- ✅ Chrome 80+
- ✅ Firefox 75+
- ✅ Safari 13+
- ✅ Edge 80+

### Performance Tips
- Use lower resolution for better performance on older devices
- Disable background removal on slower computers
- Close other browser tabs for optimal performance
- Ensure good lighting for better motion detection

## 🐛 Troubleshooting

### Common Issues

**Camera not working?**
- Ensure camera permissions are granted
- Check if camera is being used by another application
- Try refreshing the page

**No sound generated?**
- Check if "Generate Music from Motion" is enabled
- Ensure browser audio is not muted
- Try moving more dramatically to trigger motion detection

**Poor ASCII quality?**
- Increase resolution setting
- Improve lighting conditions
- Enable background removal for cleaner output

**Performance issues?**
- Lower the resolution setting
- Disable background removal
- Close other browser tabs
- Use a more powerful device

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **MediaPipe Team** - For the amazing selfie segmentation technology
- **React Team** - For the excellent frontend framework
- **Web Audio API** - For enabling real-time audio synthesis
- **ASCII Art Community** - For inspiration and techniques

## 📞 Contact & Support

- **GitHub**: [@holasoymalva](https://github.com/holasoymalva)
- **Issues**: [Report bugs or request features](https://github.com/holasoymalva/everyone_can_sound/issues)
---

<div align="center">

**Made with ❤️ by [Malva](https://github.com/holasoymalva)**

*"Where every movement becomes music, and every frame becomes art"*

[⭐ Star this project](https://github.com/holasoymalva/everyone_can_sound) if you found it interesting!

</div>
