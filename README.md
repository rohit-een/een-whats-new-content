# EEN What's New Content

PM-managed content for the VMS WebApp "What's New" in-app announcements.

## How to update

Edit `content.json` directly via the GitHub web UI and commit to `main`. The app fetches this file at runtime (cached for 1 hour).

## content.json schema

```json
{
  "version": "2026-03",          // Change this to bust the "seen" badge cache
  "pitchText": "See the latest features",
  "slides": [
    {
      "id": "unique-id",
      "type": "feature",
      "image": "https://cdn.een.com/...",   // 16:9 image URL
      "videoUrl": null,                      // or a video URL
      "title": "Feature Title",
      "bullets": ["Bullet 1", "Bullet 2"],
      "cta": {
        "primary":   { "label": "Learn more", "url": "https://..." },
        "secondary": { "label": "How to?",    "url": "https://..." }
      }
    }
  ]
}
```

## Archive

Past releases are stored in `archive/YYYY-MM.json` and used by the Releases history page.
