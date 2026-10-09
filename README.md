# Neon Reels - Slot Machine Randomizer

A modern, responsive web-based slot machine application that generates a random number within a user-defined range. It features a realistic digital "flashing" animation that decelerates over 5 seconds before locking in the final result.

## 📖 Description

This project provides a sleek, cyber-casino styled user interface where users can set an upper limit (from 0000 to 9999). Upon clicking "SPIN", the four digital reels rapidly flash random numbers, gradually slowing down over exactly 5 seconds until they land on a randomly generated number within the specified range. 

**Key Features:**
*   Strict random generation based on user input (e.g., setting `0030` will only output `0001` to `0030`).
*   5-second realistic deceleration animation (fast to slow).
*   Motion blur and neon glowing effects for an authentic digital slot machine feel.
*   Fully responsive design (works on mobile, tablet, and desktop).
*   Built entirely with vanilla web technologies (no build tools required).

## 💻 Languages Used

*   **HTML5:** Structuring the semantic layout of the application.
*   **Tailwind CSS (via CDN):** Handling all responsive styling, layout, and modern UI design (glassmorphism, gradients, shadows).
*   **Vanilla JavaScript (ES6):** Managing the state, input validation, random number generation, and the custom deceleration animation loop using `setTimeout` and `performance.now()`.
*   **CSS3:** Custom styling for the digital font, neon text shadows, and motion blur effects.

## 🚀 How to Use

### External Use (For End Users)
1. Open the website in any modern web browser (Chrome, Firefox, Safari, Edge).
2. Locate the **"Set Upper Limit"** input field.
3. Enter a 4-digit number (e.g., `0030` or `0500`). 
   * *Note: The system will automatically strip non-numeric characters.*
   * *Note: If you enter `0030`, the result will strictly be between `0001` and `0030`.*
4. Click the red **"SPIN"** button.
5. Watch the reels flash random numbers for 5 seconds as they slow down.
6. The final result will be displayed in the glowing green text below the machine.

### Internal Use (For Developers)
This project is designed to be completely plug-and-play with zero build steps.

1. **Clone or Download:** Download the source code folder to your local machine.
2. **Open the File:** Locate the main HTML file (e.g., `index.html`).
3. **Run:** Simply double-click the `index.html` file to open it in your default web browser. 
4. **Edit:** Open the file in any code editor (VS Code, Sublime Text, Notepad++). You can modify the Tailwind classes directly in the HTML for styling, or edit the `<script>` tag at the bottom for logic changes.
5. **Dependencies:** Ensure you have an active internet connection, as the project relies on the Tailwind CSS CDN (`https://cdn.tailwindcss.com`) and Google Fonts (`Share Tech Mono`).

### Customizing the Animation Speed
If you wish to change the 5-second duration, locate the following line in the `<script>` tag:
```javascript
const SPIN_DURATION = 5000; // 5000 milliseconds = 5 seconds
