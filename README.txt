BIRTHDAY UNIVERSE — ENHANCED EDITION
====================================

WHAT YOU GET
A music-synchronized 5-photo time-travel website with a realistic luminous
space portal, rotating-phone landscape guide, bundled real SVG controls (no emoji),
rose photography, floral particles, glass birthday letters and a warm finale.

QUICK SETUP
If you prefer ONE HTML file, use birthday_single_file.html (linked separately).
The multi-file package is recommended for easier development.

1) Open index.html in an editor (VS Code is recommended).
2) Put these files in the SAME folder as index.html (or change CONFIG paths):

   index.html
   blank x shout out.mp3
   1.png
   2.JPG
   3.png
   4.jpg
   5.jpg

   IMPORTANT: Filenames and capitalization must match exactly on deployment.
   The photos/ folder included here is optional; use it if you change the paths
   to photos/1.png, photos/2.JPG, etc.

3) Modify the CONFIG section near the bottom of index.html:
   - name: your girlfriend's nickname
   - subtitle: your affectionate label
   - message: your birthday wish
   - sign: closing signature
   - heroPhoto: featured photo on the surprise page
   - music: filename of your actual MP3
   - musicStart: start point in the song
   - surpriseAt: exact timestamp when the surprise should appear
   - duration: full desired progress bar duration
   - photos[]: timing, captions, file paths, tilt, entry/exit side
   - captions[]: texts shown as the five photos fly past

4) Prefer using a local server for testing (it also works as a hosted website):
   python -m http.server 5500
   Then visit: http://localhost:5500

   You can also open index.html directly in many browsers, while connected
   to the internet for the external fonts, rose photo and photo fallback.

PERFECT MUSIC SYNCHRONIZATION
- Play your real MP3 in the browser.
- Visit http://localhost:5500/?sync=1
- Click OPEN YOUR UNIVERSE.
- Press Space or MARK on the music beats you want to accent.
- Copy the collected beat timestamps into CONFIG.beats.
- Set CONFIG.surpriseAt to the EXACT second of the birthday song's drop.
- The photos, reveal and countdown all follow the music currentTime, and
  automatically catch up after a browser tab has been suspended.

PHOTO TIP
Use five compressed photos around 1200px wide / under 500 KB each for smoother
playback on mobile. Your file names must match; 2.JPG != 2.jpg on hosting.
If a file is absent, a floral stock-image fallback is shown for preview.

MOBILE / SOUND
You must tap Open to start audio; browsers prohibit unsolicited sound autoplay.
Landscape locking and full screen work on some devices, but iOS may decline.
The layout remains responsive on phones in both orientations.

HOSTING
Upload index.html, the MP3 and the 5 photo files to Cloudflare Pages,
Netlify, GitHub Pages, Vercel, or another static hosting service.

VISUAL ASSET SOURCES
- Vue 3 v3.5.13 bundled in assets/vendor/ (MIT license)
- Font Awesome Free SVG icons bundled in assets/icons/ (CC BY 4.0; attribution and license included)
  https://fontawesome.com/
- Google Fonts: Playfair Display, Great Vibes, DM Sans (open fonts)
- Real rose cut-out: Public Domain Pictures (CC0)
  https://www.publicdomainpictures.net/en/view-image.php?image=658161
- Missing photo placeholder: Unsplash floral photograph
  https://images.unsplash.com/photo-1490750967868-88aa4486c946

The font and rose image resources need an internet connection. Vue and icons
are bundled locally, and your own photos/MP3 load from your website.
No emoji artwork is used.

NOTES
Real song length and true drop timing cannot be determined without the MP3.
The initial surpriseAt=20 seconds is a starting setting copied from your code.
