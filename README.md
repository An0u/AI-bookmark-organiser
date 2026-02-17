Bookmark Organiser
An AI-powered tool that sorts your Firefox bookmarks into clean folders — no installs, no sign-ups, runs entirely in your browser.

How it works
You give it your exported bookmarks file. It sends the titles and URLs to Claude (Anthropic's AI) in batches, which assigns each one to a folder. You download the result and import it back into Firefox. Done.
All processing happens between your browser and Anthropic's API directly — nothing is stored or sent anywhere else.

Setup
1. Get a Claude API key
Go to console.anthropic.com, create an account, and generate an API key. It'll look like sk-ant-api03-...
Cost for ~2,000–3,000 bookmarks is typically under $0.10 (uses Claude Haiku, the cheapest model).
2. Export your bookmarks from Firefox

Bookmarks menu → Manage Bookmarks → Import & Backup → Export Bookmarks to HTML

Save the file somewhere you can find it (e.g. bookmarks.html on your Desktop).
3. Open bookmark-organizer.html in your browser
Just double-click the file — no server needed.
4. Follow the steps in the app

Paste your API key
Drop in your bookmarks.html
Review the folder categories (edit them if you like)
Click Organise my bookmarks
Wait for it to process (takes 1–3 minutes depending on how many bookmarks you have)
Download the result

5. Import back into Firefox

Bookmarks menu → Manage Bookmarks → Import & Backup → Import Bookmarks from HTML

Select the downloaded bookmarks-organised.html file.
