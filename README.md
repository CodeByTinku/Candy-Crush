# Candy Crush Clone 🍬

A simple, web-based clone of the popular puzzle game "Candy Crush", built using HTML, CSS, and Vanilla JavaScript.

---

## 🎮 Features
- **Classic 9x9 Grid:** A fully functional game board honoring the classic layout.
- **Drag & Drop Interactions:** Swap adjacent candies organically using the native HTML5 drag-and-drop API.
- **Match-3 Mechanics:** Automatically detects and crushes 3 consecutive matching candies horizontally or vertically.
- **Gravity & Generation:** Crushed candies leave blank spaces, causing candies above to slide down, and randomly generates new ones at the top to fill the board.
- **Scoring System:** Keeps track of points based on your successful matches.

## 🛠️ Built With
- **HTML5:** Page structure and element declarations.
- **CSS3:** Styling, grid formatting via Flexbox, and background setups.
- **Vanilla JavaScript:** All game logic, including multidimensional array tracking, event listeners for user input, match validation algorithms, and dynamic DOM updates.

## 🚀 How to Run Locally
Because this project utilizes purely static frontend development files, no server setup or dependencies are required!

1. **Download/Clone** this repository to your local machine.
2. Confirm the `images/` directory exists with all candy assets (e.g., `Blue.png`, `Orange.png`, `blank.png`) and the `background.jpg` image.
3. Open the `index.html` file in your preferred web browser (Google Chrome, Firefox, Edge, Safari).
4. Start playing and setting a high score!

## 🧩 Key Implementation Details
- **Drag Events:** Heavy utilization of `dragstart`, `dragover`, `dragenter`, `dragleave`, `drop`, and `dragend` to securely track which tiles the user is interacting with.
- **Move Validation:** The game checks if a requested swap is directly adjacent (up, down, left, right). It temporarily performs the swap, checks if it creates a valid match, and reverts it instantly if the move was invalid!
- **Game Loop:** Utilizes `window.setInterval()` running every 100 milliseconds to repeatedly trigger three core lifecycle functions: `crushCandy()`, `slideCandy()`, and `generateCandy()`.

**[🎮 Play the Live Game Here!](https://candy-crush-weld.vercel.app/)**

## 📸 Screenshots
![your device is very slow!!!](<Screenshot 2026-03-02 095021.png>)

---
*Thank you for visiting my project!*
