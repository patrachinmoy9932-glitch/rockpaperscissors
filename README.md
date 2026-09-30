# Rock Paper Scissors Game

A simple Rock Paper Scissors game built with HTML, CSS, and vanilla JavaScript. Pick rock, paper, or scissors, watch both hands shake, and see who wins against the computer.

## Live Demo

**[Play the game here](https://your-username.github.io/rock-paper-scissors/)**

## Features

- Play against a computer that picks randomly
- Shaking-hands animation before each result
- Clear result message: "User Won!!", "Cpu Won!!", or "Match Draw"
- Selected option is highlighted
- Extra clicks are blocked while a round is running
- Clean, centered card layout using the Poppins font

## Project Structure

```
rock-paper-scissors/
├── index.html      # Page structure
├── style.css       # Styling and shake animations
├── script.js       # Game logic
└── images/
    ├── rock.png
    ├── paper.png
    └── scissors.png
```

## How to Run Locally

1. Download or clone this repository:
   ```bash
   git clone https://github.com/your-username/rock-paper-scissors.git
   ```
2. Open the project folder.
3. Double-click `index.html` to open it in your browser.

No installation or build step is needed.

## How to Play

1. Click **Rock**, **Paper**, or **Scissors**.
2. Both hands shake for about 2.5 seconds.
3. The computer's choice is revealed and the winner is shown.
4. Click any option to play again.

## Game Rules

| You | CPU | Result |
|-----|-----|--------|
| Rock | Scissors | You win |
| Paper | Rock | You win |
| Scissors | Paper | You win |
| Same choice | Same choice | Draw |
| Anything else | | CPU wins |

## How It Works

- `script.js` stores each choice as `R`, `P`, or `S`, combines the user's and CPU's letters (for example `RS`), and looks up the winner in an `outcomes` object.
- The `start` class on `.container` triggers the CSS shake animation and disables clicks on the options until the round ends.
- The CPU choice is picked with `Math.floor(Math.random() * 3)`.

## Technologies Used

- HTML5
- CSS3 (Flexbox, keyframe animations)
- JavaScript (ES6)

## Deploying with GitHub Pages

1. Push the project to a GitHub repository.
2. Go to **Settings > Pages**.
3. Under **Source**, choose the `main` branch and the `/ (root)` folder, then save.
4. After a minute or two, your site will be live at `https://your-username.github.io/repository-name/`.
5. Paste that link into the **Live Demo** section above.

## Possible Improvements

- Add a score counter
- Add a reset button
- Make the layout responsive for small screens
- Add sound effects
- Add keyboard controls

## License

This project is open source and free to use for learning purposes.
