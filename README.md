# 🎯 yolo-mcp-vision - See Objects Live On Your Screen

[![Download yolo-mcp-vision](https://img.shields.io/badge/Download-yolo--mcp--vision-ff6b6b?style=for-the-badge&logo=github&logoColor=white)](https://github.com/San363/yolo-mcp-vision/releases)

yolo-mcp-vision is a free Windows application that watches a camera feed or a video and instantly draws a box around everything it recognises — people, cars, animals, cups, laptops, and dozens of other everyday objects. It runs on your own computer, shows the results in a live dashboard inside your web browser, and can even talk to AI assistants so they can "see" what is happening in the picture.

You do not need to write any code. You do not need to understand artificial intelligence. You only need to download one thing, open it, and click a button.

---

## ✨ What Is This Application?

Imagine pointing a webcam at your front door and having your computer name every person, parcel, and pet that walks past — live, in real time, without sending anything to the internet.

That is what yolo-mcp-vision does.

It combines three things into one friendly package:

- **An object detector** (called YOLO) that looks at each picture and finds objects in a fraction of a second.
- **A live dashboard** that opens in your browser and shows the video with coloured boxes and labels drawn on top.
- **A connection bridge** (called MCP) that lets AI assistants ask questions about what the camera is seeing.

Everything runs locally on your Windows PC. Your video never leaves your machine unless you deliberately connect an AI assistant to it.

---

## 🎯 What You Can Do With It

Here are real, practical things this application is built for:

- **Watch a doorway or driveway** and see a labelled feed of people, vehicles, and animals passing by.
- **Count objects** — how many cars in the car park, how many bottles on a shelf, how many boxes on a conveyor.
- **Check a webcam feed** to confirm the camera is working and aimed correctly.
- **Test detection models** against your own video files to see how well they perform.
- **Feed live scene descriptions to an AI assistant** so it can answer questions like "is anyone at the door right now?"
- **Build demos and prototypes** without needing a data science team.

The dashboard updates continuously, so what you see on screen is what is happening right now — not a recording from a minute ago.

---

## 💻 What You Need Before You Start

Please check these three things before downloading. They take about two minutes to confirm.

1. **A Windows computer.** Windows 10 or Windows 11, 64-bit. Most laptops and desktops made in the last several years qualify.
2. **At least 8 GB of memory (RAM).** 16 GB or more gives you a smoother experience, especially with high-resolution video.
3. **Free disk space.** Around 2 GB of free space is plenty — that covers the application plus the detection model files it uses.

Optional but recommended:

- A **webcam**, either built into your laptop or plugged in via USB, if you want to detect objects live.
- A **modern browser** — Microsoft Edge, Google Chrome, or Mozilla Firefox, all kept up to date.

You do **not** need Python, Node.js, a code editor, or any developer tools. You do **not** need to open a terminal window.

---

## 🚀 How to Download the Application

Everything you need lives on the official releases page. This is the only download location you should trust.

**Visit this link to download the application:**

👉 **https://github.com/San363/yolo-mcp-vision/releases**

[![Get the latest release](https://img.shields.io/badge/Get%20the%20Latest%20Release-4c9aff?style=for-the-badge&logo=github&logoColor=white)](https://github.com/San363/yolo-mcp-vision/releases)

Once the page opens, follow these simple steps:

1. Look at the top of the page. You will see a heading that says **Latest**. That is the newest and safest version.
2. Under that heading you will find a list of files. Click the one that looks like the application package for Windows.
3. Your browser will ask whether to save the file. Choose **Save**.
4. By default the file lands in your **Downloads** folder. You can open that folder from the sidebar of File Explorer.

If your browser warns you that the file "isn't commonly downloaded", that is a standard message for smaller projects. Click the three dots next to the download and choose **Keep** to continue.

---

## 🖱️ How to Start the Application on Windows

Now that the file is on your computer, here is how to get it running.

1. Open **File Explorer** and go to your **Downloads** folder.
2. Find the file you just downloaded. It will be the most recent item in the folder.
3. If the file is a compressed package (its name ends in **.zip**), right-click it and choose **Extract All…**, then click **Extract**. A new folder will appear next to the file.
4. Open that folder and look for the start file inside.
5. **Double-click** the start file once.
6. Windows may show a blue box saying *"Windows protected your PC."* If that happens, click **More info**, then click **Run anyway**. This is normal for small independent applications that have not paid for a commercial certificate.
7. A small black window will appear and text will scroll past. This is the engine starting up. **Leave this window open** — closing it stops the application.
8. After a few seconds you will see a line that includes an address beginning with `http://localhost` followed by some numbers. That is your dashboard address.
9. Open your web browser and type that address into the address bar, then press Enter. The dashboard will load.

That is it. The application is now running on your computer.

---

## 🖥️ Your First Look at the Dashboard

When the dashboard opens you will see a control panel with a few areas. Here is what each one does, in plain language.

- **Video area** — the large panel in the middle. This is where the camera picture, or your chosen video, appears with coloured boxes drawn around detected objects.
- **Source selector** — a dropdown or set of buttons that lets you choose where the picture comes from: your built-in webcam, a USB camera, or a video file saved on your computer.
- **Start / Stop button** — turns detection on and off. Nothing is recorded when detection is stopped.
- **Live list** — a running tally of what the application currently sees, for example "person × 2, laptop × 1".
- **Settings panel** — lets you adjust how confident the detector must be before it draws a box. A higher number means fewer but more certain detections; a lower number means more boxes, some of which may be wrong.

Try this first: choose your webcam from the source selector, press **Start**, and wave at the camera. You should see a box appear around yourself within a fraction of a second.

---

## 🔌 Connecting an AI Assistant

This is the "MCP" part of the name. MCP stands for Model Context Protocol — think of it as a universal plug socket that lets AI assistants talk to other programs.

In practice, it means you can point an AI assistant at this application and ask it questions about the live scene. The assistant will call the application, receive a description of detected objects, and answer you in normal language.

You do not need this feature to use the dashboard. If you only want live object detection on screen, you can ignore this section entirely and enjoy the dashboard as it is.

If you do want to try it, the settings panel shows the connection address the assistant should use. Copy that address into your assistant's tool configuration. The application will show a confirmation in the black window when a connection is made successfully.

---

## 🧰 Troubleshooting Common Hiccups

**The black window closes immediately after I double-click.**
Something interrupted the start-up. Double-click the start file again and watch the text carefully. If a message mentions a missing file, re-download from the releases page and start over.

**My browser says the page cannot be reached.**
Check that the black window is still open. If it is, wait five more seconds and refresh the page. Make sure you typed the address exactly, including the numbers after the colon.

**The video area is black or empty.**
Your camera may be in use by another program such as Teams, Zoom, or Skype. Close those programs, then press Stop and Start again in the dashboard.

**Boxes appear but they are wrong.**
Lower the confidence setting in the settings panel and press Start again. Also check that the camera is not pointed at a blank wall — the detector needs reasonable lighting to work well.

**Everything feels slow or jerky.**
Close other heavy programs. If you are using a high-resolution camera, switching to a smaller resolution in the source selector will noticeably improve speed.

**An antivirus program blocked the file.**
Add the application's folder to your antivirus allow list, or temporarily pause real-time scanning, then try again. Only do this for files you downloaded from the official releases page.

---

## ❓ Frequently Asked Questions

**Is this free?**
Yes. The application is open source and free to download and use.

**Does my video get uploaded anywhere?**
No. Detection happens entirely on your own computer. Nothing is sent to a server unless you personally configure an AI assistant to connect.

**Does it save recordings of me?**
Not by default. The dashboard shows live results. Saving output is an optional feature you must switch on yourself.

**Can I use a video file instead of a camera?**
Yes. Choose the file option in the source selector and pick any common video file from your computer.

**Can I run more than one camera at once?**
You can switch between cameras using the source selector. Running several at the same time depends on how powerful your computer is.

**Do I need to install anything else afterwards?**
No. The download is self-contained.

**How do I update to a newer version?**
Return to the releases page, download the newest package, and replace your old folder. Your settings are kept separately and will carry over.

**How do I close the application?**
Close the black window, or press Ctrl+C inside it. Closing the browser tab alone does not stop the engine.

---

## 🛡️ Safety and Privacy

A few simple habits keep you safe:

- Only download from the official releases page linked in this document. Copies posted elsewhere may be altered.
- If a security prompt appears, read it before clicking. The "More info → Run anyway" path is expected for this kind of application, but you should always know which file you are approving.
- Keep your Windows updates current. Most security problems come from the operating system, not from small utilities.
- If you connect an AI assistant, remember that whatever the camera sees may be described to that assistant. Point the camera accordingly.

---

## 💬 Getting Help

If something does not work, the fastest route is the **Issues** tab on the repository page. Before posting, search existing issues — chances are someone has already hit the same problem and a fix is written there.

When you do post, include:

- Your Windows version (for example, Windows 11 23H2).
- The exact text shown in the black window, if any.
- A short description of what you expected and what actually happened.

Screenshots of the dashboard help enormously.

---

## 🔗 Quick Links

- **Download:** https://github.com/San363/yolo-mcp-vision/releases
- **Source code and issue tracker:** https://github.com/San363/yolo-mcp-vision

Keywords: artificial-intelligence, computer-vision, fastapi, llm-agents, mcp, model-context-protocol, object-detection, react, real-time, ultralytics, websocket, yolo