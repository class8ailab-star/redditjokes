Cure Depression? 🎭

An ultra-minimalist, immersive web app designed to cycle through Reddit jokes with fluid transitions, dynamic typography, and ambient environmental effects.

✨ Features

Ultra-Minimalist Interface: Starts completely dark and empty with only a centered, subtle button.

Dynamic Typography: Automatically analyzes the length of the joke or setup and dynamically adjusts font sizes, line heights, and weights so it always looks stunning on both desktop and mobile screens.

Visual Distinction:

The Setup (Title): Rendered in a cool, soft ice-blue with a subtle back-glow aura and an indigo HUD badge.

The Punchline (Body): Transitions into a rich, energetic emerald-mint green with a matching ambient background glow.

Offline/Local Fail-safe: Includes a built-in troubleshooter. If the browser blocks local file fetching (CORS policy), it provides an instant in-browser dashboard to paste your raw JSON and play immediately.

📂 File Structure

For this project to work, keep both files in the same folder:

my-joke-app/
├── index.html     # The web application
└── jokes.json     # Your dataset of Reddit jokes


jokes.json Format

Ensure your JSON file is formatted as an array of objects like this:

[
  {
    "id": "5tz52q",
    "score": 1,
    "title": "I hate how you cant even say black paint anymore",
    "body": "Now I have to say \"Leroy can you please paint the fence?\""
  },
  {
    "id": "6ax73b",
    "score": 12,
    "title": "What's the best thing about Switzerland?",
    "body": "I don't know, but the flag is a big plus."
  }
]


🚀 How to Run Locally

Because modern browsers restrict local file reading (fetch()) when opening HTML files directly from your file system (using the file:/// protocol), you need a quick local server to run this app properly.

Method 1: Using Python (Recommended)

Open your terminal or command prompt.

Navigate to your project folder:

cd path/to/my-joke-app


Run the built-in Python server:

Python 3: python -m http.server 8000

Python 2: python -m SimpleHTTPServer 8000

Open your browser and go to: http://localhost:8000

Method 2: VS Code "Live Server"

Open your project folder in Visual Studio Code.

Install the Live Server extension (by Ritwick Dey).

Click the "Go Live" button in the bottom-right corner of the VS Code window.

Method 3: No-Server Fallback

If you don't want to run a server right now, simply open the index.html file in your browser. The app's built-in troubleshooter will appear, allowing you to copy-paste the contents of your jokes.json directly into the text box to start playing instantly.

🌐 Deployment

When you are ready to share this with the world, you can host it for free on platforms like GitHub Pages, Vercel, or Netlify. Since they serve your files over a secure network, the database fetch will work flawlessly out of the box!
