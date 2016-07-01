uEye
----
A micro-lib for UI/UX interaction recording, logging & playback (IE9+) _(MIT Licensed)_

---
#### Have you ever wondered...

- How do users interact with my website/SPA?
- How well does it load/perform for them?
- What are they doing before bouncing?
- Do they bother scrolling the landing pages? How far?
- What UI path leads to the fastest or highest value conversions?

uEye can help you answer these and other questions without relying on third-party analytics libs (which can be slow, bulky and ad-blocked) and without compromising your users' privacy.

---
#### Features

- Tiny - 2k recorder, 2k player
- Unobtrusive & fast - uses events' capture phase and 100ms polling
- Simple API for recording, playback & extending
- Custom event logging
- Chrome, Firefox, IE9+ (recorder), Chrome, Firefox (player)
- 0 dependencies, though the following are recommended, as needed:
	- [simpleheat](https://github.com/mourner/simpleheat) for heatmaps
	- [hammer.js](https://github.com/hammerjs/hammer.js) for touch & gesture events
	- [mousetrap](https://github.com/ccampbell/mousetrap) for key combo events
	- [keycode](https://github.com/timoxley/keycode) for keycode mapping
	- [JSONH](https://github.com/WebReflection/JSONH) for log compression
	- [alite](https://github.com/chrisdavies/alite) for ajax

---
#### Usage

---
#### Demos

---
#### Docs

---
#### Limitaions

- uEye does not simulate mouse/keyboard/touch events (this is often impossible), so will not interact with your web page besides scrolling and resizing. The lib only shows when & where the events occur. For example, if a user hovers a drop-down nav menu or types into a form field, this will not visually occur during playback. However, if you've logged these events you can hook the player's `onevent` and manually trigger these actions as you see fit.
- The player does not yet support multiple logs, so it's limited to replaying interactions with only a single page. To replay a user's entire session, you would need to string together multiple logs, though this should be fairly simple.

---
#### TODO