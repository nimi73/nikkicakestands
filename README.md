
# Nikki Cake Stands - Developer Guide

## How to Change Images

All images and videos in this app are managed in one central file:
`src/lib/placeholder-images.json`

### Option 1: Use a URL (Current Method)
Simply replace the `imageUrl` string with any `https://...` link.

### Option 2: Use Local Files (Recommended for Production)
1. Place your image file (e.g., `my-stand.jpg`) into the `public/` folder.
2. In `src/lib/placeholder-images.json`, set the `imageUrl` to the relative path:
   ```json
   "imageUrl": "/my-stand.jpg"
   ```

### Option 3: Base64
You can use a Base64 encoded string as the `imageUrl`:
   ```json
   "imageUrl": "data:image/png;base64,iVBORw0KG..."
   ```

## Tech Stack
- Next.js 15 (App Router)
- React 19
- Tailwind CSS
- Genkit (AI Inquiry Assistant)
- Lucide React (Icons)
