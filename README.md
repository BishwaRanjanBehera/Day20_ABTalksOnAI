# Day20_ABTalksOnAI - Output
Day20_ABTalksOnAI

Here's the complete face puzzle game — a single self-contained HTML file with:

Camera capture: getUserMedia() with front camera, live preview, snapshot to canvas, graceful permission-denied/no-camera/insecure-context error handling with a Retry button
Puzzle generation: 3×3/4×4/5×5 selection, image sliced via CSS background-position/size per tile, randomized (always solvable since it's a free swap-based puzzle, not a sliding puzzle)
Drag & drop: unified mouse + touch handlers, snap-to-nearest-cell on release, pink border while dragging, green border when a piece is correctly placed
Timer/moves: live mm:ss.t timer, move counter, correct-piece tally, all updating in real time
Win detection: auto-detects full solve, stops timer, shows results overlay, saves top 5 times to localStorage with date/time/moves/difficulty, renders a leaderboard
UI: Retake Photo, New Photo, Reshuffle/Play Again buttons, responsive layout for mobile and desktop, dark modern theme

Just open the file in a browser over HTTPS or localhost — camera access requires a secure context.

<img width="632" height="627" alt="image" src="https://github.com/user-attachments/assets/fd0446d7-76cd-4973-999c-1b6f56163e64" />

file:///C:/Users/bishw/Downloads/face_puzzle.html

🧩 Built a fully functional Face Puzzle Game — entirely in a single HTML file, zero frameworks.

The challenge: take a photo via webcam, turn it into a sliding puzzle, and make it feel polished on both desktop and mobile — all client-side, no backend, no dependencies beyond the browser itself.

What it does:
📸 Requests webcam access and lets you snap a live selfie
🧩 Slices the photo into a 3×3, 4×4, or 5×5 grid and scrambles it
🖱️ Full drag-and-drop support — mouse and touch — with snap-to-grid and visual feedback (highlighted borders while dragging, green borders on correct placement)
⏱️ Live timer + move counter + real-time "pieces correct" tracker
🏆 Auto win-detection, a results screen, and a persistent top-5 leaderboard saved in localStorage
📱 Responsive, clean UI that works across Chrome, Firefox, and Safari

The fun part was handling the edge cases: graceful fallback when camera permissions are denied, HTTPS/localhost requirements for getUserMedia(), and making drag gestures feel smooth and identical across mouse and touch events without any external libraries.

A nice reminder that you don't always need a heavy framework — vanilla JS, CSS, and the Canvas/MediaDevices APIs can get you surprisingly far.

#WebDevelopment #JavaScript #FrontEnd #BuildInPublic #100DaysOfCode





