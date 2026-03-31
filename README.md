# 📦 Sokoban: James the Laborant

A classic **Sokoban-style puzzle game** built with a modern web stack. Help James, the dedicated lab assistant, organize the warehouse by pushing crates into their designated slots.

-----

## 🎮 How to Play

1.  **Objective:** Move all wooden crates onto the pink **"X"** target tiles.
2.  **Controls:** Use your **Keyboard Arrow Keys** ($\uparrow \downarrow \leftarrow \rightarrow$) to move James.
3.  **Pushing:** Walk into a crate to push it.
4.  **The Rules:**
      * You can only push **one crate** at a time.
      * Crates cannot be pulled.
      * Crates cannot pass through walls or other crates.
      * The level is cleared only when *every* target tile is covered by a crate.

-----

## 🚀 Features

  * **Progressive Difficulty:** 3 unique levels ranging from a simple $3 \times 3$ tutorial to a complex $5 \times 6$ warehouse with 6 crates.
  * **Animated UI:** Smooth CSS transitions for character movement and box sliding.
  * **Visual Feedback:** Crates glow and scale up when successfully placed on a target.
  * **Responsive Logic:** Robust collision detection prevents clipping through walls or overlapping objects.
  * **Modern Aesthetic:** A "Dark Lab" theme with high-fidelity icons and 3D depth shadows.

-----

## 🛠 Project Structure

```text
├── soko_maze.html      # Game structure & UI containers
├── soko_maze.js        # Game Engine (OOP logic, movement, & collision)
├── soko_maze.css       # Graphical styles (compiled from SCSS)
└── README.md           # Documentation
```

### Technical Stack

  * **HTML5 / CSS3 (SCSS):** Advanced layouts and keyframe animations.
  * **JavaScript (ES6+):** Object-Oriented approach using Classes for `Player`, `Box`, and `Map`.
  * **jQuery:** Efficient DOM manipulation and keyboard event handling.
  * **Bootstrap 5:** Modal styling and layout utilities.

-----

## 🔧 Installation & Setup

1.  **Clone the repository** (or download the files).
2.  **Dependencies:** Ensure you are connected to the internet. The project loads **jQuery** and **Bootstrap** via CDN.
3.  **Run:** Open `soko_maze.html` in any modern web browser (Chrome, Firefox, Edge).

> **Note:** If you are modifying the styles, ensure you compile the `.scss` file into `.css`, or link a Sass-compiler in your workspace.

-----

## 📝 Level Configurations

  * **Level 1:** Introduction to movement and single-box pushing.
  * **Level 2:** Introduces multi-box management and tighter corners.
  * **Level 3:** The "Grand Master" level—requires precise planning to avoid "locking" crates against walls.

-----

## 🧪 Developer Notes

The game logic is encapsulated in a `GameEngine` class. To add a new level, simply append a new object to the `LEVELS` array in `soko_maze.js`:

```javascript
{
    size: { x: Width, y: Height },
    player: { x: startX, y: startY },
    boxes: [{ start: { x: bx, y: by }, end: { x: tx, y: ty } }]
}
```

-----

**Happy Pushing\!** 🧪📦