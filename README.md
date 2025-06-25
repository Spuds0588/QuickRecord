# QuickRecord
### The Instant Screen Recorder Bookmarklet

[![Website](https://img.shields.io/badge/Website-View_Live-blue?style=for-the-badge)](https://spuds0588.github.io/QuickRecord/)
[![Buy Me A Coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-Donate-yellow?style=for-the-badge&logo=buymeacoffee)](https://buymeacoffee.com/burnsdevelopment)

QuickRecord is a powerful, zero-installation screen and webcam recorder that lives entirely in your browser. It solves the problem of clunky, slow-to-install software by giving you an instant recording tool right in your bookmarks bar.

It's perfect for developers reporting bugs, support teams creating tutorials, or anyone who needs to capture their screen without the hassle of a traditional application.



## ✨ Features

*   **🎥 Screen + Webcam Recording:** Capture your entire screen with a picture-in-picture webcam overlay to add a personal touch.
*   **🖱️ Zero Installation:** It's just a bookmarklet. No software, no browser extensions, and no admin rights needed.
*   **🚀 Instant & Fast:** Click the bookmark and the recorder opens in a new tab, ready to go in seconds.
*   **🔒 100% Private & Secure:** All recording and processing happens locally in your browser. Your data never touches a server, ensuring complete privacy.
*   **🎤 Audio Capture:** Records your microphone input alongside your screen and camera.
*   **⬇️ Immediate Download:** Get a high-quality `.webm` video file the moment you stop recording.

## 🚀 Getting Started in 10 Seconds

Installation is as simple as dragging a link to your bookmarks bar.

1.  **Go to the QuickRecord Website:**
    ### [https://spuds0588.github.io/QuickRecord/](https://spuds0588.github.io/QuickRecord/)

2.  **Drag the Button:**
    Find the main call-to-action button and simply **drag and drop it** onto your browser's bookmarks bar.

3.  **Click to Record:**
    That's it! Navigate to any page, click your new "QuickRecord" bookmark, and start recording.

## ❤️ Support the Project

If you find QuickRecord useful and want to say thanks, please consider supporting my work. It helps me dedicate more time to creating and maintaining helpful open-source tools like this one!

<a href="https://buymeacoffee.com/burnsdevelopment" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

## 🛠️ How It Works (Under the Hood)

QuickRecord leverages modern browser APIs to provide a seamless experience without relying on any backend servers.

*   **`navigator.mediaDevices.getDisplayMedia`**: Used to capture the screen content.
*   **`navigator.mediaDevices.getUserMedia`**: Used to capture webcam and microphone streams.
*   **HTML5 `<canvas>`**: The screen and webcam video streams are drawn onto a hidden canvas in real-time to composite them into a single picture-in-picture view.
*   **`MediaRecorder API`**: This powerful API takes the stream from the canvas, encodes it into a `.webm` video file, and provides the data chunks for download.

The entire application—HTML, CSS, and JavaScript—is Base64 encoded and embedded directly into the bookmarklet's `javascript:` URL. When clicked, it opens a new window and writes the decoded HTML to it, effectively creating a self-contained web app on the fly.

## 📝 License

This project is open source and available under the [MIT License](LICENSE).
