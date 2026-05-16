# 🖤 Morticia — Memorial Website

A living memorial for **Morticia**, our beloved black Indian Lab. 2 June 2021 – 4 March 2026.

## Pages

| Page | File | Purpose |
|------|------|---------|
| Home | `index.html` | Hero, intro, story previews |
| About | `about.html` | Who she was, her facts |
| Stories | `stories.html` | All memory stories |
| Gallery | `gallery.html` | Photo albums by year |
| Timeline | `timeline.html` | Life milestones |
| Scrapbook | `scrapbook.html` | Doodles, videos, keepsakes |

## How to add content

### Add a photo
1. Upload image to `assets/photos/`
2. In `gallery.html`, replace a placeholder `<div class="gallery-item">` with:
```html
<div class="gallery-item fade-in">
  <img src="assets/photos/YOUR-FILE.jpg" alt="Description" />
</div>
```

### Add a story
1. Duplicate `stories/first-day.html` → rename it
2. Fill in the title, date, author, and body text
3. Add a card for it in `stories.html`

### Add a timeline milestone
In `timeline.html`, add a new block inside `.timeline`:
```html
<div class="timeline-item fade-in">
  <div class="timeline-dot"></div>
  <div class="timeline-year">Month Year</div>
  <div class="timeline-event">What happened</div>
  <div class="timeline-desc">A sentence about this moment.</div>
</div>
```

### Add a scrapbook item
1. Upload scanned image to `assets/doodles/`
2. In `scrapbook.html`, add:
```html
<div class="scrapbook-item fade-in">
  <img src="assets/doodles/YOUR-FILE.jpg" alt="Description" class="scrapbook-img" />
  <div class="scrapbook-caption">Your caption in Caveat handwriting style</div>
</div>
```

### Embed a video
1. Upload to Google Drive → Share → Anyone with link
2. Copy the File ID from the URL
3. In `scrapbook.html`, add the iframe embed (see comments in the file)

## Structure

```
/
├── index.html
├── about.html
├── stories.html
├── gallery.html
├── timeline.html
├── scrapbook.html
├── css/
│   └── style.css
├── js/
│   └── main.js
├── assets/
│   ├── photos/
│   ├── videos/
│   └── doodles/
└── stories/
    └── first-day.html    ← template
```

---

*Good girls live forever.* 🐾
