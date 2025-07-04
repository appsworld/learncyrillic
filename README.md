# Cyrillic Space Defense

Cyrillic Space Defense is a browser based educational game that helps users learn the Russian Cyrillic alphabet. You defend Earth by matching falling Cyrillic letters or letter combinations with their Latin equivalents and pronunciations. The project runs entirely in the browser and uses the Web Speech API for audio feedback.

## Features

* Interactive learning grid that plays the natural pronunciation of each letter
* Game mode with falling asteroid like characters that move toward Earth
* Progressive difficulty: single letters, two character combinations, three character combinations
* Adjustable falling speed: slow, normal, fast, extreme
* Score, streak and level tracking
* Keyboard and mouse input
* Pronunciation playback through Web Speech API with graceful fallback to visual cues
* Polished visual design including starfield background, glowing effects and particle explosions
* Responsive layout that works on desktop and mobile

## Quick Start

1. Clone or download this repository.
2. Open `index.html` in a modern browser that supports the Web Speech API.
3. Select Learn First to review the alphabet or choose a game mode to start playing.

You can also serve the project with a simple static server:

```bash
npx serve .
```

## Gameplay

### Learning Mode

* Click any letter card to hear its pronunciation and see phonetic hints.

### Easy Mode

* Asteroids containing single Cyrillic letters fall toward Earth.
* Click a Latin option or press the matching key to destroy the asteroid.
* Maintain a streak to unlock two character combinations.

### Challenge Mode

* Asteroids fall faster and include the full alphabet from the start.
* The game unlocks longer combinations more quickly.

During any game you can:

* Change falling speed with the Speed buttons.
* Switch between character modes with the Characters buttons once unlocked.
* Pause the audio by pressing another answer button or by waiting for playback to finish.

The game ends when you lose all lives. Your final score and learning progress appear in a modal dialog.

## File Structure

```
index.html     Main file that holds HTML, CSS and JavaScript
```

All logic, styles and assets are in a single file for simplicity. You may split them into separate files if you plan to extend the project.

## Customization

* Edit the `cyrillicData` array to change transliterations, phonetics or sample words.
* Adjust animation timing in `getAnimationDuration`.
* Replace images or backgrounds by editing the relevant CSS blocks.

## Browser Support

The game requires a browser that supports both ES6 and the Web Speech API. It works in recent versions of Chrome, Edge and Firefox. Some voices may vary between platforms.
