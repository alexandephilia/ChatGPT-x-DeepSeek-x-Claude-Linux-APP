# AI Chat Desktop Applications
![image](https://github.com/user-attachments/assets/29bc20ee-56bd-46f5-b5a3-43603723a7a7)

This repository contains Electron-based desktop applications for various AI chat platforms. Each application is designed to provide a native desktop experience for web-based AI chat services. 

> Contributors: Alexandephilia x Sonnet 3.5

## Repository Structure

```
electron_app/
├── ChatGPT_APP/       # Electron wrapper for ChatGPT
├── DeepSeek_APP/      # Electron wrapper for DeepSeek Chat
├── Claude_APP/        # Electron wrapper for Claude AI
└── Grok_APP/          # Electron wrapper for Grok
```

## Applications

### ChatGPT_APP

![image](https://github.com/user-attachments/assets/82b3de05-4881-4442-96f3-456c4ce13d80)


An Electron-based desktop application for ChatGPT.

**Key Files:**
- `main.js` - Main Electron process that creates windows and handles system integration
- `renderer.js` - Renderer process script that interacts with the ChatGPT web interface
- `preload.js` - Preload script that bridges the main and renderer processes
- `package.json` - Project configuration and dependencies
- `chatgpt.png` - Application icon
- `dist/` - Build output directory

**Features:**
- System tray integration
- Hardware acceleration for better performance
- Media access for voice input
- Single instance lock to prevent multiple instances

![image](https://github.com/user-attachments/assets/5031c1be-9230-4f4b-9228-fd80a450ec00)

> NOTE: **Voice mode and clipboard functionality fully working!**

### Claude_APP

![image](https://github.com/user-attachments/assets/14593cce-422b-40a4-8bec-7fd8554af96c)


An unofficial Electron wrapper for Claude AI desktop application.

**Key Files:**
- `README.md` - Detailed documentation about the Claude desktop application
- `build-deb.sh` - Script to build a Debian package for the application
- `LICENSE-APACHE` and `LICENSE-MIT` - Dual license files
- `.gitignore` - Git ignore configuration

**Features:**
- MCP (Model Control Protocol) support
- System tray integration
- Cross-platform compatibility with Linux focus

![image](https://github.com/user-attachments/assets/d135a9b6-e92e-451f-a579-a1c0f2d0f35a)

> NOTE: - **Quick shortcut chat with Ctrl+Alt+Space** for instant access anywhere


### DeepSeek_APP

An Electron wrapper for DeepSeek Chat.

![image](https://github.com/user-attachments/assets/80c92bbb-d6dd-4171-a383-7447242edb1c)

**Key Files:**
- `main.js` - Main Electron process
- `package.json` - Project configuration and dependencies
- `DEEP_SEEK.png` - Application icon
- `dist/` - Build output directory containing the AppImage and other build artifacts
- `node_modules/` - Node.js dependencies

**Features:**
- System tray integration
- Persistent session for login state
- Permission handling for web content
- Cross-platform build configuration


### Grok_APP

![image](https://github.com/user-attachments/assets/f6f8b27a-085c-49b0-8671-2e6bec62ff71)

An Electron-based desktop application for Grok.

**Key Files:**
- `main.js` - Main Electron process that creates windows and handles system integration
- `renderer.js` - Renderer process script that interacts with the Grok web interface
- `preload.js` - Preload script that bridges the main and renderer processes
- `package.json` - Project configuration and dependencies
- `chatgpt.png` - Application icon
- `dist/` - Build output directory

**Features:**
- System tray integration
- Hardware acceleration for better performance
- Media access for voice input
- Single instance lock to prevent multiple instances

## Building and Running

Each application can be built and run independently:

### ChatGPT_APP

```bash
cd ChatGPT_APP
npm install
npm start     # Run the application
npm run build # Build the application
```

### Claude_APP

```bash
cd Claude_APP
sudo ./build-deb.sh # Build a Debian package
sudo dpkg -i ./build/electron-app/claude-desktop_*.deb # Install the package
```

### DeepSeek_APP

```bash
cd DeepSeek_APP
npm install
npm start     # Run the application
npm run build # Build the application
```

### Grok_APP

```bash
cd Grok_APP
npm install
npm start     # Run the application
npm run build # Build the application
```

## License

- ChatGPT_APP, Grok_APP and DeepSeek_APP: Refer to their respective package.json files
- Claude_APP: Dual-licensed under MIT and Apache License 2.0

## Notes

These applications are wrappers around web-based services and may be subject to the terms of service of their respective platforms. They are designed to enhance the user experience by providing native desktop integration features. 
