# Bookmark Organiser

An AI-powered tool that sorts your Firefox bookmarks into clean folders — no installs, no sign-ups, runs entirely in your browser.

---

## How it works

You give it your exported bookmarks file. It sends the titles and URLs to Claude (Anthropic's AI) in batches, which assigns each one to a folder. You download the result and import it back into Firefox. Done.

All processing happens between your browser and Anthropic's API directly — nothing is stored or sent anywhere else.

---

## Setup

**1. Get a Claude API key**

Go to [console.anthropic.com](https://console.anthropic.com), create an account, and generate an API key. It'll look like `sk-ant-api03-...`

Cost for ~2,000–3,000 bookmarks is typically **under $0.10** (uses Claude Haiku, the cheapest model).

**2. Export your bookmarks from Firefox**

> Bookmarks menu → Manage Bookmarks → Import & Backup → Export Bookmarks to HTML

Save the file somewhere you can find it (e.g. `bookmarks.html` on your Desktop).

**3. Open `bookmark-organizer.html` in your browser**

Just double-click the file — no server needed.

**4. Follow the steps in the app**

- Paste your API key
- Drop in your `bookmarks.html`
- Review the folder categories (edit them if you like)
- Click **Organise my bookmarks**
- Wait for it to process (takes 1–3 minutes depending on how many bookmarks you have)
- Download the result

**5. Import back into Firefox**

> Bookmarks menu → Manage Bookmarks → Import & Backup → Import Bookmarks from HTML

Select the downloaded `bookmarks-organised.html` file.

---

## Default folders

| Folder | What goes in it |
|---|---|
| 🎨 Design | UX/UI, Figma, design systems, inspiration |
| 📋 Product Management | Roadmaps, agile, PM resources |
| 💻 Development | Coding, GitHub, dev tools, APIs |
| 💼 Work & Career | Job hunting, interviews, LinkedIn |
| 📚 Learning & Courses | Online courses, tutorials, books |
| 📰 Articles & Reading | Blogs, newsletters, read-later |
| 🛍️ Shopping | Etsy, Amazon, clothing, gear |
| 🏋️ Health & Fitness | Nutrition, sports, wellness |
| 💰 Finance | Investing, banking, budgeting |
| 🎬 Entertainment | Streaming, music, games |
| 🔧 Tools & Productivity | SaaS tools, utilities, apps |
| 🌿 Personal & Hobbies | Crafts, sewing, personal projects |
| ✈️ Travel | Flights, hotels, trip planning |
| 👥 Social & Community | Forums, Reddit, communities |
| 📌 Other | Anything that doesn't fit |

You can see and edit these before the AI runs.

---

## Privacy

- Your API key is used only to call Anthropic's API and is never stored
- Only bookmark **titles and domain names** are sent to the API (not full URLs)
- Bookmark icons and metadata stay local
- Nothing is saved between sessions

---

## Troubleshooting

**"Invalid API key"** — Make sure your key starts with `sk-ant-` and has no extra spaces.

**Batches failing** — Usually a temporary API issue. Bookmarks from failed batches go into "Other" — you can re-run the tool on just those if needed.

**Import shows duplicates** — Firefox merges on import, so existing bookmarks won't be deleted. You may want to clear your old bookmarks first (export a backup first just in case).

**Some bookmarks landed in the wrong folder** — AI categorisation isn't perfect. For bulk moves, use Firefox's built-in bookmark manager after importing.
