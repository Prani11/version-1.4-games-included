# Sonora

Sonora is a responsive music player and movie-song guessing game built with HTML, CSS, vanilla JavaScript, and Bootstrap 5.3.8.

## Run it

Open `index.html` in a modern browser. For the best experience, run the folder from a small local web server (for example, VS Code Live Server). An internet connection is needed for Bootstrap, Google Fonts, artwork, iTunes Search, and audio previews.

## What's included

- Responsive top navigation for Home, Search, Library, and Games
- Language selection for Telugu, Hindi, English, Tamil, Malayalam, Kannada, Korean, and Japanese
- Curated movie-song quiz questions with multiple-choice answers, verification, correct-answer reveal, score, and next-round progression
- Existing-style music controls: play/pause, next/previous, shuffle, repeat, seek, volume, liked songs, and iTunes search
- Responsive sign-in page at `login.html` (authentication is a front-end placeholder)

## Catalog and game limitations

The game question and movie association are curated in `script.js`; the answer is not inferred from catalog search results. Sonora searches the public iTunes Search API for a preview whose title and artist match the curated entry. Catalog coverage can vary by country and time. If no plausible match or no preview is available, the question remains playable and the interface explains that audio is unavailable for that round. iTunes previews are short samples, not full tracks, and network or browser policy can prevent them from playing.

The general music player searches iTunes for playable song previews. Results depend on the catalog and internet access. Liked tracks are saved in the browser's local storage. Account forms do not create accounts or authenticate users until connected to a back end.

## Files

- `index.html` — music player and game interface
- `style.css` — responsive theme and layouts
- `script.js` — catalog playback, saved likes, navigation, and quiz logic
- `login.html` — sign-in and create-account placeholder
