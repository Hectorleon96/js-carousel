# Boring Vanilla Carousel 🎡

A production-ready, fully responsive carousel built with pure **Vanilla JS, HTML5, and CSS3** in less than 100 lines of code. No React, no component libraries, no `npm install`, and absolutely zero framework black magic.

I was bored, so I decided to skip the modern bundle-bloat and remind everyone how the web actually works when you dominate the fundamentals.

## The "Framework Magic" Breakdown

To anyone who can't manage state without an external engine, here is your breakdown:

- **Your React Context / Redux Store:**
  ```javascript
  let visibleIndex = 0;
  let autoplayIntervalId = undefined;
  ```
- **Your Virtual DOM Reconciliation:**
  A highly optimized, hardware-accelerated CSS translation.
  ```javascript
  carouselItems.style.transform = `translateX(-${visibleIndex * 100}%)`;
  ```
- **Your Custom Hooks / Event Handlers:**
  A single memory-efficient Event Delegation listener directly on the parent DOM.

## Features

- **Mathematical Responsiveness:** Moves on the X-axis using relative percentages (`%`), automatically adapting to any viewport size without listening to window resize events.
- **Smart Autoplay:** Automatically resets its own interval timer on manual user interaction to prevent abrupt slide changes.
- **Real Persistence:** Remembers user preferences natively via `localStorage`.
- **High Performance:** Uses a single event listener for the entire component instead of clogging the browser's RAM with individual button event handlers.

## How to use

1. Double click on `index.html`.
2. That's it. No `npm install`, no `npm run dev`, no local server needed.

---

_Built out of pure boredom to demystify front-end abstractions._
