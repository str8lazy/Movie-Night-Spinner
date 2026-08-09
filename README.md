# Movie Night Spinner 🎬 🎲

A stylish web-based movie selector that helps groups decide what to watch. Simply input movie suggestions from family and friends, spin the wheel, and let fate decide your next movie night pick!

## Features

- Interactive spinning wheel animation
- Cyberpunk-inspired design with glowing effects
- Easy-to-use interface for adding movie entries
- Celebratory winner announcement with visual effects
- Responsive layout that works on various screen sizes
- Persistent winner history displayed in stylish walls on either side of the wheel
- Dedicated **Winner History** edit page (`edit.html`) to edit, remove, or clear past winners
- Undo / redo for history edits (toolbar and keyboard shortcuts)
- Export and upload winner history as JSON (with size and schema safety checks)

## How to Use

1. Open the application in your web browser (`wheel.html`)
2. Enter movie suggestions in the text area (one movie per line)
3. Click the "Spin" button to start the wheel
4. Watch as the wheel spins and randomly selects a movie
5. The winning movie will be displayed in a stylish popup overlay
6. Open **Edit History** to manage saved winners, export a backup, or upload a JSON file

### Editing winner history

1. From the spinner, click **Edit History** (or open `edit.html`)
2. Edit movie names and dates inline, or remove individual winners
3. Use **Undo** / **Redo** if you change your mind (`Ctrl/Cmd+Z`, `Ctrl/Cmd+Shift+Z` or `Ctrl/Cmd+Y`)
4. **Export JSON** downloads `movie-night-winners.json`
5. **Upload JSON** replaces the current history after confirmation (max 1MB; validated schema)

## Technical Details

Built using vanilla:
- HTML5
- CSS3 (with modern animations and effects)
- JavaScript (for wheel animation, interaction, and saving history with `localStorage`)

No external dependencies or installation required - just open the HTML file in a modern web browser.

Winner history is stored under the `movieNightWinners` key in `localStorage` and shared between `wheel.html` and `edit.html`.

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/movie-night-spinner.git
   ```

2. Open the `wheel.html` file in your web browser
3. Start adding movies and spinning!

## Browser Support

Works best in modern browsers that support:
- CSS Grid and Flexbox
- CSS Animations and Transitions
- Canvas API
- Modern JavaScript (ES6+)
- File API (for JSON upload/export on the edit page)

## License

MIT License - feel free to use and modify as needed!
