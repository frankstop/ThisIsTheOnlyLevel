# This Is The Only Level (Web Implementation)

A faithful recreation of the classic puzzle-platformer where the level layout stays the same, but the rules and mechanics change every time you play. Built using HTML5 Canvas, Tailwind CSS, and vanilla JavaScript.

---

## 🕹️ Gameplay
You control a small elephant trying to reach the green pipe. While the physical layout of the level never changes, each stage introduces a "twist" that forces you to rethink your approach.

### 🔗 Live Demo
Play the game here: [https://frankstop.github.io/ThisIsTheOnlyLevel/](https://frankstop.github.io/ThisIsTheOnlyLevel/)

### Features
* **6 Unique Stages:** Including reversed controls, invisibility, and meta-puzzles.
* **Retro Aesthetics:** Uses the "Press Start 2P" font and 8-bit color palette for a classic arcade feel.
* **Physics Engine:** Custom collision detection for platforms, spikes, and interactive triggers.
* **Responsive Design:** Styled with Tailwind CSS to ensure the game container fits various screen sizes.

---

## 🛠️ Technical Implementation

### Core Components
* **Game Loop:** Uses `requestAnimationFrame` with a 60 FPS cap to ensure smooth movement across different monitors.
* **State Machine:** A centralized `setupLevel()` function manages the transition between stages, resetting player position and modifying game rules (e.g., toggling `player.visible`).
* **Collision Detection:** * **AABB (Axis-Aligned Bounding Box):** Used for platforms and goal detection.
    * **Spike Logic:** Custom rendering and hit-box logic for hazard areas.
* **Meta Elements:** The game interacts with DOM elements outside the canvas (like the page title) to solve specific puzzles.

### Controls
| Key | Action |
| :--- | :--- |
| **Arrow Left** | Move Left |
| **Arrow Right** | Move Right |
| **Arrow Up** | Jump / Fly |

---

## 🚀 Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/frankstop/ThisIsTheOnlyLevel.git
    ```
2.  **Run the game:**
    Simply open the `index.html` file in any modern web browser, or visit the [GitHub Pages site](https://frankstop.github.io/ThisIsTheOnlyLevel/).

---

## 📂 Project Structure
* `index.html`: Contains the game logic, rendering engine, and styles in a single-file portable format.
* `Tailwind CSS`: Handled via CDN for layout and responsive utility classes.
* `Google Fonts`: Pulls "Press Start 2P" for the retro typography.

---

## 📝 License
This project is open-source and available under the MIT License.
