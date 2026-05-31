# Markdown Live Preview

> A professional, lightweight web-based Markdown editor with real-time live preview, advanced syntax support, and dark mode.

[![License: ISC](https://img.shields.io/badge/License-ISC-yellow.svg)](https://opensource.org/licenses/ISC)
[![GitHub Stars](https://img.shields.io/github/stars/Alisha-21-cloud/markdown-live-preview)](https://github.com/Alisha-21-cloud/markdown-live-preview)
[![Live Demo](https://img.shields.io/badge/Demo-Live-brightgreen)](https://markdown-live-preview-coral.vercel.app/)

## 🎯 Overview

**Markdown Live Preview** is a powerful, minimal web-based Markdown editor designed for writers, developers, and documentation creators. It provides an intuitive split-panel interface with real-time synchronization, allowing you to write Markdown on one side and see the formatted output instantly on the other. With support for advanced features like Mermaid diagrams, customizable themes, and local storage persistence, this tool is perfect for quick drafts, documentation, and learning Markdown syntax.

## ✨ Features

### Core Features
- **Live Preview** - See your Markdown rendered in real-time as you type
- **Split-Panel Editor** - Side-by-side editing and preview interface
- **Syntax Highlighting** - Professional code highlighting with Monaco Editor
- **Dark Mode** - Built-in dark and light theme support with persistent storage
- **Synchronized Scrolling** - Optional scroll sync between editor and preview panes

### Advanced Capabilities
- **Mermaid Diagram Support** - Create beautiful diagrams and flowcharts directly in Markdown
- **GitHub Markdown Styling** - Uses authentic GitHub-flavored Markdown CSS for consistent styling
- **Code Block Support** - Syntax highlighting for multiple programming languages
- **PDF Export** - Export your Markdown as PDF documents
- **Copy to Clipboard** - Easy one-click copying of rendered HTML
- **Local Data Persistence** - Your work is automatically saved to browser's local storage
- **Sanitized HTML** - XSS protection using DOMPurify for safe rendering

### User Experience
- **Responsive Design** - Works seamlessly on desktop and tablets
- **Resizable Panels** - Drag to adjust editor and preview pane widths
- **Reset Function** - Clear and start fresh with a single click
- **Default Template** - Includes comprehensive Markdown syntax guide for learning

## 🚀 Live Demo

Experience Markdown Live Preview now: **[https://markdown-live-preview-coral.vercel.app/](https://markdown-live-preview-coral.vercel.app/)**

## 📋 Supported Markdown Syntax

- **Headers** - H1 through H6
- **Text Formatting** - Bold, italic, strikethrough, and combinations
- **Lists** - Ordered, unordered, and nested lists
- **Code Blocks** - Inline code and code blocks with language-specific syntax highlighting
- **Links & Images** - Full support with alt text and titles
- **Tables** - Multi-column tables with alignment options
- **Blockquotes** - Single and nested blockquotes
- **Horizontal Rules** - Visual content separators
- **Mermaid Diagrams** - Flowcharts, sequence diagrams, Gantt charts, and more

## 🛠️ Technology Stack

### Frontend
- **Editor** - [Monaco Editor](https://microsoft.github.io/monaco-editor/) v0.52.2 (VS Code's powerful editor)
- **Markdown Parser** - [Marked.js](https://marked.js.org/) v15.0.7
- **Diagrams** - [Mermaid](https://mermaid.js.org/) v11.15.0
- **Styling** - [GitHub Markdown CSS](https://github.com/sindresorhus/github-markdown-css) v5.8.1
- **Security** - [DOMPurify](https://github.com/cure53/DOMPurify) v3.4.0 (XSS protection)
- **Storage** - [Storehouse.js](https://github.com/tanabe/Storehouse-js) (Local storage wrapper)

### Build & Development
- **Build Tool** - [Vite](https://vitejs.dev/) v6.4.2 (Fast frontend tooling)
- **Package Manager** - npm

## 📦 Installation

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Quick Start

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Alisha-21-cloud/markdown-live-preview.git
   cd markdown-live-preview
   ```

2. **Install Dependencies**
   ```bash
   make setup
   # or manually
   npm install
   ```

3. **Start Development Server**
   ```bash
   make dev
   # or manually
   npm run dev
   ```

4. **Open in Browser**
   Open your browser and navigate to `http://localhost:5173` (or the URL shown in terminal)

## 🔨 Development

### Available Commands

**Setup & Installation**
```bash
make setup          # Install all dependencies
npm install         # Alternative: install dependencies
```

**Development**
```bash
make dev            # Start Vite development server with hot reload
npm run dev         # Alternative command
```

**Build for Production**
```bash
make build          # Build optimized production bundle
npm run build       # Alternative command
```

**Preview Production Build**
```bash
make preview        # Preview the production build locally
npm run preview     # Alternative command
```

**Serve Production Build**
```bash
npm run serve-dist          # Serve the dist folder on port 5001
npm run build-and-serve     # Build and serve in one command
```

## 📁 Project Structure

```
markdown-live-preview/
├── src/
│   └── main.js                 # Application entry point & main logic
├── public/
│   ├── css/
│   │   ├── style.css          # Main application styles
│   │   ├── github-markdown-light.css    # Light theme styles
│   │   └── github-markdown-dark_dimmed.css  # Dark theme styles
│   ├── image/                 # Static images and assets
│   ├── 404.html              # 404 error page
│   └── favicon.png           # App favicon
├── index.html                 # HTML entry point
├── package.json              # Project dependencies & scripts
├── vite.config.js            # Vite configuration
├── firebase.json             # Firebase configuration
├── Makefile                  # Build automation commands
├── LICENSE                   # ISC License
└── README.md                 # This file
```

## 💾 Data Persistence

All your edits are automatically saved to your browser's **local storage** under the namespace `com.markdownlivepreview`. This includes:
- **last_state** - Your Markdown content
- **scroll_bar_settings** - Scroll synchronization preference
- **theme_settings** - Your selected theme (light/dark)

Your data persists between sessions and is only lost when you clear browser data or click the reset button.

## 🎨 Customization

### Themes
- **Light Mode** - Clean, readable design with white background
- **Dark Mode** - Eye-friendly dark theme with reduced strain
- Toggle between themes using the "Dark mode" checkbox in the header

### Editor Customization
The application comes with a built-in Markdown syntax guide as the default template. You can clear this and start with your own content at any time.

## 🔐 Security

- **XSS Protection** - All HTML rendering is sanitized using DOMPurify to prevent injection attacks
- **Client-Side Processing** - All markdown processing happens in your browser; no data is sent to servers
- **No Cookies** - The app doesn't use cookies; only local storage on your device

## 📱 Browser Compatibility

Works with all modern browsers that support:
- ES6+ JavaScript
- Local Storage API
- CSS Grid & Flexbox
- Monaco Editor

**Recommended Browsers:**
- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## 🚀 Deployment

This project is deployed on **Vercel** and automatically updates on every push to the main branch.

### Deploy Your Own Version

**Option 1: Deploy to Vercel (Recommended)**
1. Fork this repository on GitHub
2. Connect your fork to Vercel
3. Vercel will automatically build and deploy on every push

**Option 2: Deploy to Firebase Hosting**
```bash
npm install -g firebase-tools
firebase login
firebase deploy
```

**Option 3: Static Hosting**
```bash
npm run build
# Upload the `dist/` folder to your hosting provider (GitHub Pages, Netlify, etc.)
```

## 📖 Usage Examples

### Basic Markdown
```markdown
# Hello World

This is **bold** and this is *italic*.

- Item 1
- Item 2
  - Nested item
```

### Code Example
```markdown
### Code Example
\`\`\`javascript
function greet(name) {
  return `Hello, ${name}!`;
}
\`\`\`
```

### Mermaid Diagram
```markdown
\`\`\`mermaid
graph TD
  A[Start] --> B{Decision}
  B -->|Yes| C[Success]
  B -->|No| D[Retry]
\`\`\`
```

## 🤝 Contributing

Contributions are welcome! To contribute:

1. **Fork the Repository**
   ```bash
   git clone https://github.com/Alisha-21-cloud/markdown-live-preview.git
   cd markdown-live-preview
   ```

2. **Create a Feature Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make Your Changes**
   - Follow the existing code style
   - Test your changes thoroughly

4. **Commit & Push**
   ```bash
   git add .
   git commit -m "Add: description of your changes"
   git push origin feature/your-feature-name
   ```

5. **Open a Pull Request**
   - Describe your changes clearly
   - Link any related issues

## 🐛 Bug Reports & Feature Requests

Found a bug or have a feature idea? Please [open an issue](https://github.com/Alisha-21-cloud/markdown-live-preview/issues) on GitHub.

## 📄 License

This project is licensed under the **ISC License**. See the [LICENSE](./LICENSE) file for details.

## 🔗 Links

- **Live Demo** - https://markdown-live-preview-coral.vercel.app/
- **GitHub Repository** - https://github.com/Alisha-21-cloud/markdown-live-preview
- **Issue Tracker** - https://github.com/Alisha-21-cloud/markdown-live-preview/issues

### Special Thanks
- [Marked.js](https://marked.js.org/) - Markdown parser
- [Monaco Editor](https://microsoft.github.io/monaco-editor/) - Editor component
- [Mermaid](https://mermaid.js.org/) - Diagram support
- [GitHub Markdown CSS](https://github.com/sindresorhus/github-markdown-css) - Styling
- [DOMPurify](https://github.com/cure53/DOMPurify) - Security

## 📞 Support

If you need help or have questions:
- Check the [GitHub Issues](https://github.com/Alisha-21-cloud/markdown-live-preview/issues) for similar problems
- Review the default Markdown syntax guide in the app
- Open a new issue with detailed information about your problem

---

**⭐ If you find this project helpful, please consider giving it a star on [GitHub](https://github.com/Alisha-21-cloud/markdown-live-preview)!**
