# Resonate

A personal vocal coach that runs in the browser. It tracks your pitch live through the microphone and takes you from beginner to advanced through 25 scored lessons.

## Features
- **Live pitch tracking** (YIN algorithm): a scrolling pitch graph, a target band and a cents meter showing how flat or sharp you are
- **Curriculum**
  - Beginner: breathing, hiss support, range finder, pitch matching, 5-note scale, sirens, steady notes, higher/lower ear test
  - Intermediate: major scale, arpeggios, thirds, interval ear training, octave sirens, steady sustain, singing a tune back from memory
  - Advanced: messa di voce, vibrato analysis, chromatic scale, wide leaps, agility runs, range extension, all intervals, ±15-cent precision, longer tunes from memory
- **Personalised**: exercises are pitched to your measured range
- **Progress**: stars, day streak, minutes practised and a daily warm-up. Saved in your browser (localStorage).
- **Tuner** for free singing, with reference notes

No build step and no dependencies. Everything is in `index.html`.

## Running it
The browser only gives a page access to the microphone when the page is served securely (https or `localhost`).

**On your computer**
```bash
git clone https://github.com/MitchOwenss/Resonate.git
cd Resonate
python3 -m http.server 8000
# open http://localhost:8000 in your browser
```

**On your phone** (GitHub Pages, https)
1. Turn on Pages: repo **Settings → Pages → Source: GitHub Actions**. Pages works on private repos only with a paid GitHub plan (Pro, Team or Enterprise).
2. Every push to `main` deploys the app to `https://mitchowenss.github.io/Resonate/`.
3. Open that address in Safari or Chrome and choose **Add to Home Screen** to install it like an app.

## Tips
- Use headphones so the guide tones don't leak into the mic.
- Open vowels ("ah", "oo") and humming track best.
- Stop if anything hurts or feels hoarse.
