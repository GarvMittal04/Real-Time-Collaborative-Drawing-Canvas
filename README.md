# 🎨 Collaborative Drawing Canvas (Flam Assignment)

> A real-time multiplayer drawing app where creativity meets collaboration!

## 🌐 Live Demo

**[✨ Try it live here!](https://your-app-url.onrender.com)** ← Replace with your actual URL

Open it in multiple tabs and watch the magic happen! 🪄

---

## 💡 What is this?

Ever wanted to draw with friends in real-time, no matter where they are? That's exactly what this app does! 

Think of it like Google Docs, but for drawing. Multiple people can draw on the same canvas simultaneously, and everyone sees the changes instantly. It's perfect for:

- 🎓 Remote teaching and tutoring
- 🎮 Playing Pictionary with friends
- 💼 Collaborative brainstorming sessions
- 🎨 Just having fun doodling together!

---

## ✨ Cool Features

### 🖌️ Drawing Tools
- **Brush**: Draw smooth, colorful strokes
- **Eraser**: Fix your mistakes (we all make them!)
- **Color Picker**: Choose from millions of colors
- **Brush Size**: From tiny details (1px) to bold strokes (50px)

### 👥 Collaboration Magic
- **Real-time Sync**: See others draw as they draw, not after!
- **User Colors**: Each person gets a unique color identifier
- **Live Cursors**: See where others are pointing (like in Figma)
- **User List**: Know who's online with you

### 🔄 Advanced Stuff
- **Global Undo/Redo**: Anyone can undo the last action (democratic art! 🗳️)
- **Clear Canvas**: Start fresh (with everyone's permission)
- **Performance Monitor**: See your FPS counter (for the nerds 🤓)
- **Touch Support**: Draw with your finger on mobile/tablet

### ⌨️ Keyboard Shortcuts
Because who doesn't love shortcuts?
- `Ctrl/Cmd + Z`: Undo
- `Ctrl/Cmd + Y` or `Ctrl/Cmd + Shift + Z`: Redo

---

## 🚀 Running It Yourself

Want to tinker with the code? Here's how!

### What You Need
- **Node.js** (version 14 or newer) - [Download here](https://nodejs.org/)
- A terminal/command prompt
- 5 minutes of your time ⏱️

### Installation
```bash
# 1. Clone this repository (or download the ZIP)
git clone https://github.com/YOUR_USERNAME/collaborative-canvas.git

# 2. Go into the folder
cd collaborative-canvas

# 3. Install dependencies (this might take a minute)
npm install

# 4. Start the server
npm start
```

That's it! Open `http://localhost:3000` in your browser. 🎉

### Testing with Multiple Users

Want to test the collaboration feature?

**Easy way:**
1. Open `http://localhost:3000` in Chrome
2. Open `http://localhost:3000` in Firefox (or another Chrome tab)
3. Start drawing in one → watch it appear in the other! ✨

**Impress your friends:**
1. Find your computer's IP address:
   - **Windows**: Open CMD, type `ipconfig`, look for "IPv4 Address"
   - **Mac/Linux**: Open Terminal, type `ifconfig`, look for "inet"
2. Share `http://YOUR_IP:3000` with friends on the same WiFi
3. Now you're all drawing together! 🎨

---

## 📁 Project Structure
```
collaborative-canvas/
├── client/                  # Frontend (what you see in the browser)
│   ├── index.html          # The main page structure
│   ├── style.css           # Makes it look pretty 💅
│   ├── canvas.js           # Handles all the drawing logic
│   ├── websocket.js        # Talks to the server in real-time
│   └── main.js             # Brings everything together
│
├── server/                  # Backend (the brain of the operation)
│   ├── server.js           # Main server file
│   ├── rooms.js            # (Future) Multiple room support
│   └── drawing-state.js    # Manages the drawing history
│
├── package.json            # List of dependencies
└── README.md               # You are here! 👋
```

---

## 🎯 How It Works (Simple Explanation)

1. **You draw** → Your browser captures the pen movements
2. **Message sent** → "Hey server, I drew a line from (10,20) to (30,40)"
3. **Server broadcasts** → "Everyone! Someone drew a line!"
4. **Others receive** → All connected users get the message
5. **They draw too** → Their browsers draw the same line
6. **Result**: Everyone sees the same thing! 🎉

It's like a group chat, but instead of sending text, you're sending drawing instructions!

---

## 🐛 Known Limitations

I'm being honest here - this is a learning project, not a billion-dollar app (yet 😉):

1. **Drawing History**: Doesn't save when you close the page or restart the server
2. **Undo Chaos**: If you undo, it removes the *last* thing drawn, even if someone else drew it (democracy in action!)
3. **User Limit**: Works great with 2-5 users, gets a bit laggy with 10+
4. **No Authentication**: Anyone with the link can join (good for demos, not for private stuff)
5. **Browser Support**: Works best on modern browsers (sorry, Internet Explorer fans!)

---

## 🎓 What I Learned Building This

This project taught me:
- How WebSockets enable real-time communication
- Managing state across multiple clients is HARD
- Canvas API is powerful but unforgiving
- Network latency is the enemy of smooth drawing
- Testing with yourself in multiple browser tabs feels lonely 😅

**Time spent**: About 8-10 hours
- Planning architecture: 1 hour
- Server setup: 2 hours  
- Canvas drawing engine: 2 hours
- WebSocket client: 1.5 hours
- Making it look decent: 1.5 hours
- Debugging weird edge cases: 2 hours (the real MVP 🏆)

---

## 🚀 Deployment

This app is deployed on **Render.com** (free tier). 

**Why Render?**
- ✅ Free hosting (with some limitations)
- ✅ Easy GitHub integration
- ✅ Supports WebSockets (crucial for real-time stuff)
- ✅ Auto-deploys when you push to GitHub

**Note**: Free tier apps "sleep" after 15 minutes of inactivity. They wake up in ~30 seconds when someone visits. If you want 24/7 uptime, use a service like [UptimeRobot](https://uptimerobot.com) to ping it every 5 minutes.

---

## 🤝 Want to Contribute?

Found a bug? Have an idea? Feel free to:
- Open an issue on GitHub
- Submit a pull request
- Send me a message

Some ideas for improvements:
- [ ] Save/load drawings
- [ ] Add more tools (rectangle, circle, text)
- [ ] Private rooms with passwords
- [ ] Export canvas as PNG
- [ ] Replay drawing history (timelapse!)
- [ ] Add layers (like Photoshop)

---

## 🙏 Acknowledgments

- **HTML5 Canvas API** - For making drawing possible
- **WebSocket Protocol** - For the real-time magic
- **Express.js** - For the simple server setup
- **Coffee ☕** - For keeping me awake during debugging sessions

---

## 📝 License

MIT License - Feel free to use this for learning, projects, or showing off to friends!

---

## 📧 Questions?

If you're stuck or just want to chat about the project, feel free to reach out!

**Built with ❤️ and a lot of console.log() statements**

---

**⭐ If you found this useful, consider giving it a star on GitHub!**

---

*Last updated: [Current Date]*

