# Dynamic Clock

A simple GitHub Pages web app that displays a live clock, date and scheduled messages/colours.

## Run locally

Open `index.html` in a browser.

## Change the schedule

Open `index.html` and edit the `SCHEDULE` array near the top of the `<script>` section:

```js
const SCHEDULE = [
  { time: "07:00", background: "#2563eb", text: "#ffffff", message: "Good morning" },
  { time: "12:00", background: "#eab308", text: "#111827", message: "Lunch time" }
];
```

Each entry is active from its time until the next scheduled time.

Times are interpreted using the viewer's local timezone by default. To force a timezone, set:

```js
const TIME_ZONE = "Europe/London";
```

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload `index.html` and this README.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`.
6. Save.
7. GitHub will provide the public Pages URL.

No server or database is required.
