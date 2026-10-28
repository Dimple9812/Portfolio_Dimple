# Dimple Yadav · Portfolio

**Live site:** https://dimple-yadav-portfolio.vercel.app

An interactive portfolio for a Java / Spring Boot and MERN full stack engineer. The hero is a "portfolio tree": its leaves are letters from the word PORTFOLIO and its eight fruits are my main projects. Drag the tree, click it, press **S** or use **Shake the tree** to make the letter-leaves blow off in the wind.

## What's on the page

- **Work:** 8 main projects with metrics, tech stack, live demo and GitHub links (MarketFlow, MeshPay, ReferBoard, CodeSage AI, Distributed Ticket Booking, TeamOS, CanvasHub, Cloud Storage)
- **Smaller builds:** CINÉPOP (3D popcorn site), SCAIMS, Fitness Tracker, Train Ticket Booking, To-Do List
- **Experience:** Jellyfish Technologies, Harman Connected Services (client: Mercedes-Benz)
- **Skills, education and certifications, contact**

## Tech

One self-contained `index.html`: HTML, CSS and vanilla JavaScript, with no framework and no build step.

- The tree is drawn on a `<canvas>`, with about 640 letter sprites pre-rendered once for smooth 60fps animation.
- The sway uses a damped spring that bends the tree rather than rotating it, and each fruit swings like a damped pendulum.
- The canvas is sharp on retina screens (devicePixelRatio, capped at 2) and resizes with a ResizeObserver.
- Respects `prefers-reduced-motion`; the fruits are keyboard-focusable links with labels.
- Fonts: Instrument Serif (Google Fonts) and Satoshi (Fontshare).

## Editing

Projects live in two arrays at the top of the `<script>` in `index.html`:

- `PROJECTS`: the 8 fruits and main project cards (title, tag, position on the tree, colours, links, metrics, stack)
- `MORE`: the smaller builds row

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Deploy

It's a static site. Import this repo into Vercel (framework: Other, no build command), or turn on GitHub Pages for the `main` branch.

## Contact

- Email: dimple98y@gmail.com
- LinkedIn: https://www.linkedin.com/in/dimple-yadav-1273861b5/
- GitHub: https://github.com/Dimple9812
