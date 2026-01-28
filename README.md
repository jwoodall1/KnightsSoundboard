# Knights Soundboard

A modern, responsive web-based soundboard application with two separate sections for organizing and playing audio files. Features include dynamic button management, file upload, and persistent storage.

## Link

**  https://jwoodall1.github.io/KnightsSoundboard/

## Features

- **Two Independent Sections**: Organize your sounds into two separate sections
- **Dynamic Button Management**: Add/remove buttons from each section with simple controls
- **File Upload**: Easy drag-and-drop or click-to-upload for audio files
- **Persistent Storage**: All data is automatically saved to browser's local storage
- **Save/Load Projects**: Export and import your soundboard configurations
- **Modern UI**: Beautiful, responsive design with smooth animations
- **Audio Controls**: Play sounds with visual feedback and proper audio management
- **Cross-Platform**: Works on desktop and mobile devices

## Quick Start

### Option 1: Direct File Opening
1. Open `source/index.html` in your web browser
2. Start adding buttons and uploading sounds!

### Option 2: Local Development Server (Recommended)
1. Install Node.js (if not already installed)
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```
   or for live reloading:
   ```bash
   npm run dev
   ```

## How to Use

### Adding Buttons
- Click the "➕ Add Button" button in either section to create a new sound button
- Each section can have up to 20 buttons
- Use "➖ Remove Button" to remove the last button from a section

### Uploading Sounds
- Click on an empty button (shows "Upload Sound")
- Select an audio file from your computer
- The button will update to show the sound is ready to play
- Supported formats: MP3, WAV, OGG, M4A, and other web-compatible audio formats

### Playing Sounds
- Click any button with a sound to play it
- Visual feedback shows when a sound is playing
- Only one sound per button can play at a time

### Saving Your Work
- Click "💾 Save Changes" to save your current configuration
- Data is automatically saved to your browser's local storage
- Your work persists between browser sessions

### Loading Projects
- Click "📁 Load Project" to import a previously exported soundboard
- This allows you to share configurations or backup your work

## Technical Details

### File Structure
```
KnightsSounboard/
├── source/
│   ├── index.html      # Main HTML structure
│   ├── styles.css      # CSS styling and animations
│   └── script.js       # JavaScript functionality
├── package.json        # Node.js dependencies
└── README.md          # This file
```

### Browser Compatibility
- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

### Storage
- Uses browser's Local Storage for persistence
- Data includes button configurations and audio file data
- No server required - everything runs client-side

## Customization

### Adding More Sections
To add more sections, modify the HTML structure in `index.html` and update the JavaScript in `script.js` to handle additional sections.

### Changing Button Limits
Modify the `maxButtons` property in the `sections` object in `script.js`.

### Styling
All styles are in `styles.css`. The app uses CSS Grid and Flexbox for responsive layouts.

## 🔧 Development

### Prerequisites
- Node.js 14+ (for development server)
- Modern web browser

### Available Scripts
- `npm start` - Start development server
- `npm run dev` - Start with live reloading
- `npm run serve` - Start simple HTTP server
- `npm run build` - No build process needed

## Mobile Support

The application is fully responsive and works on mobile devices. Touch interactions are supported for all button operations.

## Troubleshooting

### Audio Not Playing
- Ensure your browser supports HTML5 audio
- Check that audio files are in supported formats
- Some browsers require user interaction before playing audio

### Data Not Saving
- Check if local storage is enabled in your browser
- Ensure you have sufficient storage space
- Try clearing browser cache and reloading

### File Upload Issues
- Ensure audio files are in supported formats
- Check file size (very large files may cause issues)
- Try refreshing the page and uploading again

## License

MIT License - feel free to modify and distribute as needed.

## Contributing

This is a simple project, but contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

---
