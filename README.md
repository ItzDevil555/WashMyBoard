# 🧼 WashMyBoard (WMB)

A sleek, ultra-modern, and minimalist web application designed to let you wipe, spray, and deep-clean your physical computer keyboard without triggering accidental clicks, system shortcuts, or chaotic blocks of text. 

Built with pure HTML, CSS, and vanilla JavaScript, **WashMyBoard** locks down your browser window into full-screen mode and safely intercepts keys as you clean, turning your wiping motions into a satisfying, visual canvas of pressed keys.

[Features](#-key-features) • [How to Use](#-how-to-use) • [Under the Hood](#-how-it-works) • [Tech Stack](#-tech-stack)

---

## ✨ Key Features

*   **Aggressive Key Interception:** Neutralizes standard web browser hotkeys (such as `Tab` navigation, `Spacebar` scrolling, and `F1-F12` menus) so wiping your keys doesn't disrupt anything.
*   **Safety-Hold Escape Exit:** Prevents the app from instantly closing if you accidentally rub over the `Escape` key. Users must **hold `Esc` down for 2 continuous seconds** to exit.
*   **Immersive Fullscreen Mode:** Automatically requests full-screen mode upon launching to remove desktop and browser UI clutter for an optimal cleaning environment.
*   **Modern White Minimalist UI:** Designed with a premium, soft light-mode aesthetic, featuring crisp typography, subtle shadows, and bouncy pop-in key animations.
*   **Zero Installation:** Runs entirely client-side. No node_modules, no dependencies, no tracking.

---

## 🚀 How to Use

### Option 1: Run Locally (Fastest)
1. **Download** or copy the `index.html` file from this repository.
2. **Double-click** the file to open it in any modern web browser (Chrome, Edge, Safari, or Firefox).
3. Click the **"Start Cleaning"** button to lock the board and enter full-screen.
4. Clean away!

### Option 2: Host via GitHub Pages
1. Go to your repository settings on GitHub.
2. Scroll down to the **Pages** section on the left sidebar.
3. Under **Build and deployment**, set the source to `Deploy from a branch` and select `main` (or `master`).
4. Click **Save**. Your site will be live at `https://yourusername.github.io/your-repo-name/` in a few moments.

> 💡 **To Exit & Unlock:** Once you are finished cleaning, simply press and **hold the `Esc` key for 2 full seconds**. Your browser will exit fullscreen and your keys will unlock.

---

## 🛠️ How It Works (The Sandbox Limitation)

WMB works by utilizing the browser's `pointer-events` and `preventDefault()` event listeners during the capturing phase. 

⚠️ **Please Note on OS-Level Keys:** Because web browsers run inside a secure sandbox environment, it is physically impossible for *any* website to block global Operating System shortcuts (like the `Windows Key`, `Mac Command Key`, `Ctrl+Alt+Del`, or `Alt+Tab`). WashMyBoard successfully blocks 100% of the keys the browser legally allows it to intercept.

---

## 💻 Tech Stack

*   **HTML5** (Semantic structure)
*   **CSS3** (Custom properties, Flexbox, custom keyframe animations)
*   **Vanilla JavaScript** (Fullscreen API, Keydown tracking & event capturing)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE). Feel free to modify, break, or clean your keyboard with it however you like!
