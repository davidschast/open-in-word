# open-in-word

A one-page relay for the PoetryDB Submissions app.

The app runs inside the Claude iPhone app, which won't hand `ms-word:` links to the Word app. It will open an ordinary web page, though. So the app's **Open in Word** button opens this page with the Word link in the `#fragment`, and the page passes it on to Word.

- The page holds no data. The link travels in the fragment, which browsers never send to GitHub's servers.
- It only accepts Office "open document" links (`ms-word:` / `ms-excel:` / `ms-powerpoint:`) that point at personal OneDrive (`https://d.docs.live.net/...`). Anything else shows "Nothing to open".
