# Daily Scrum Organizer

A modern, lightweight, and fully client-side web application to help you prepare and organize your Daily Scrum/Stand-up meetings. Built with vanilla JavaScript, Tailwind CSS, and zero backend dependencies.

![Daily Scrum Organizer](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![No Dependencies](https://img.shields.io/badge/dependencies-none-brightgreen.svg)

## ✨ Features

### 📝 Core Functionality
- **Three-question format**: Yesterday, Today, and Blockers - the classic Scrum format
- **Mood indicator**: Express how you're feeling with emoji mood selection
- **Real-time preview**: See your formatted daily as you type
- **Two output formats**: Rich (with headers) and Slack-friendly formatting
- **Markdown rendering**: Beautiful preview with full Markdown support

### ⏱️ Speaking Timer
- Configurable countdown timer (default: 2 minutes)
- Visual progress bar with color indicators
- Audio/visual alert when time is up
- Quick presets: 1min, 2min, 3min

### 🏷️ Quick Tags
- Pre-configured tags like `[CR]`, `[WIP]`, `[BLOCKED]`, `[DEPLOY]`
- Fully customizable: add, edit, delete, and color-code your tags
- One-click insertion into any field
- Persistent storage of custom tags

### 📜 History
- Automatically save your dailies
- Browse past entries with date/time stamps
- Load previous dailies with one click
- Delete individual entries or clear all history
- Import "Today" from your last daily as "Yesterday"

### 🌍 Internationalization (i18n)
- **Portuguese (Brazil)** - Default
- **English**
- **Spanish**
- Easy to extend with additional languages

### ⚙️ Settings
- **Preview mode**: Expanded modal or new browser tab
- **Timer duration**: Customize default speaking time
- **Auto-save draft**: Never lose your work
- **Language selection**: Switch UI language instantly

### 🎨 User Experience
- **Dark/Light mode**: Automatic system detection + manual toggle
- **Responsive design**: Works on desktop, tablet, and mobile
- **Keyboard shortcuts**: ESC to close modals
- **Copy to clipboard**: One-click copy for pasting into Slack/Teams
- **Native share**: Share via mobile device's share sheet
- **Export/Import**: Backup and restore all your data as JSON

## 🚀 Getting Started

### Option 1: Direct Use
Simply open `daily.html` in any modern web browser. No server required!

```bash
# Clone the repository
git clone https://github.com/yourusername/daily-scrum-organizer.git

# Open in browser
open daily.html
# or
xdg-open daily.html  # Linux
start daily.html     # Windows
```

### Option 2: Host on GitHub Pages
1. Fork this repository
2. Go to Settings → Pages
3. Select "Deploy from a branch" → main → / (root)
4. Your app will be available at `https://yourusername.github.io/daily-scrum-organizer/daily.html`

### Option 3: Any Static Hosting
Upload `daily.html` to any static hosting service:
- Netlify
- Vercel
- AWS S3
- Google Cloud Storage
- Any web server

## 📖 Usage

### Basic Workflow
1. **Select your mood** using the emoji buttons
2. **Fill in your three sections**:
   - What you did yesterday
   - What you'll do today
   - Any blockers or impediments
3. **Preview** your formatted output in real-time
4. **Copy** to clipboard or **Share** directly
5. **Save** to history for future reference

### Using Quick Tags
1. Click on the text field where you want to insert a tag
2. Click any tag button in the tags bar
3. The tag will be inserted at your cursor position

### Importing Yesterday
Click "Use previous 'Today' as 'Yesterday'" to automatically populate yesterday's field with your last saved "Today" entry.

### Timer
1. Click **Start** to begin the countdown
2. Timer shows visual progress with color changes
3. Alerts you when time is up
4. Click **Reset** to start over

## 🔧 Configuration

### Customizing Tags
1. Click the **Tags** button in the navbar
2. Add new tags with custom text, label, and color
3. Edit or delete existing tags
4. Click "Restore Default" to reset to original tags

### Changing Language
1. Click **Settings** (Config) in the navbar
2. Select your preferred language
3. The UI updates instantly

### Adjusting Timer
1. Open Settings
2. Enter duration in seconds (30-600)
3. Or use quick preset buttons

## 💾 Data Storage

All data is stored locally in your browser using `localStorage`:

| Key | Description |
|-----|-------------|
| `dailyScrumDraft` | Current unsaved draft |
| `dailyScrumHistory` | Saved dailies (max 30) |
| `dailyScrumCustomTags` | Your custom tags |
| `dailyScrumSettings` | App preferences |
| `dailyScrumTheme` | Dark/light mode preference |

### Export/Import
- **Export**: Click the export button to download a JSON backup
- **Import**: Click import and select a previously exported file

## 🛠️ Technical Details

### Built With
- **Vanilla JavaScript** - No framework dependencies
- **Tailwind CSS** (via CDN) - Utility-first styling
- **Font Awesome 6** (via CDN) - Icons
- **Google Fonts (Inter)** - Typography
- **marked.js** (via CDN) - Markdown parsing

### Browser Support
- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

### File Structure
```
daily-scrum-organizer/
├── daily.html      # Single-file application
├── README.md       # This file
└── LICENSE         # MIT License
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Ideas for Contributions
- Additional language translations
- New color themes
- Integration with project management tools
- Voice input support
- Calendar integration

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by the Scrum methodology and daily stand-up best practices
- Built for developers and teams who value simplicity
- Thanks to the open-source community for the amazing tools

---

**Made with ❤️ for Agile teams everywhere**

*If you find this useful, please consider giving it a ⭐ on GitHub!*
