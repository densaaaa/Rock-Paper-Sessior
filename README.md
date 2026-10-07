# 🎮 Rock Paper Scissors Game

A simple **Rock Paper Scissors** game built with **HTML, CSS, and Vanilla JavaScript**.

The player chooses Rock, Paper, or Scissors, and the computer randomly selects its choice. JavaScript then compares both choices and displays the winner while keeping track of the score.

## 🚀 Live Demos

👉 Add your GitHub Pages link here after deployment.

## 📸 Preview

Add a screenshot of your game here:

```markdown
![Rock Paper Scissors Preview](./screenshot.png)
```

## ✨ Features

* 🪨 Rock
* 📄 Paper
* ✂️ Scissors
* 🤖 Random computer choice
* 🏆 Winner detection
* 🤝 Draw detection
* 📊 User and computer score tracking
* 🎨 Dynamic result messages
* 🖱️ Click-based gameplay
* ⚡ Built with Vanilla JavaScript

## 🛠️ Technologies Used

* **HTML5** — Structure of the game
* **CSS3** — Styling and layout
* **JavaScript (ES6)** — Game logic and DOM manipulation

## 🧠 How the Game Works

1. The player clicks one of the three choices.
2. JavaScript gets the player's choice using the element's `id`.
3. The computer randomly selects:

   * Rock
   * Paper
   * Scissors
4. The player's choice is compared with the computer's choice.
5. The game determines whether:

   * You win
   * Computer wins
   * Game is a draw
6. The score is updated after each round.
7. A message is displayed showing the result.

### Winning Rules

| Player      | Beats       |
| ----------- | ----------- |
| 🪨 Rock     | ✂️ Scissors |
| 📄 Paper    | 🪨 Rock     |
| ✂️ Scissors | 📄 Paper    |

If both players choose the same option, the game is a **draw**.

## 📂 Project Structure

```text
Rock-Paper-Scissors/
│
├── index.html
├── style.css
├── script.js
└── screenshot.png
```

## 💻 JavaScript Concepts Practiced

This project helped practice several important JavaScript concepts:

* Variables
* Functions
* Arrow functions
* `if...else`
* Ternary operator
* Arrays
* `Math.random()`
* `Math.floor()`
* DOM selection
* `querySelector()`
* `querySelectorAll()`
* `getAttribute()`
* `innerText`
* `addEventListener()`
* `forEach()`
* Template literals
* Event handling
* Basic game logic

## 🔑 Example

The computer's choice is generated randomly:

```javascript
const compChoice = () => {
    const options = ["rock", "paper", "sessor"];
    const random = Math.floor(Math.random() * 3);

    return options[random];
};
```

The player can then start a round by clicking a choice:

```javascript
choices.forEach((choice) => {
    choice.addEventListener("click", () => {
        const userChoice = choice.getAttribute("id");
        playGame(userChoice);
    });
});
```

## 📚 What I Learned

Through this project, I practiced connecting **JavaScript with HTML elements** and learned how user interactions can trigger JavaScript functions.

I also practiced breaking a program into smaller functions such as:

* `compChoice()`
* `drawGame()`
* `showWinner()`
* `playGame()`

This makes the code easier to understand and maintain.

## 🔮 Future Improvements

Possible improvements for future versions:

* 🔄 Add a **Reset Game** button
* 🏆 Add a **Best of 5** mode
* 📱 Improve mobile responsiveness
* 🎵 Add sound effects
* ✨ Add animations
* 🏅 Add win percentage/statistics
* 🌙 Add dark/light mode
* 💾 Store high scores using `localStorage`

## 👨‍💻 Author

**Irbaz Abid**

BS Computer Science Student
Aspiring Full-Stack Developer

* GitHub: [@irbaz-abid](https://github.com/irbaz-abid)

---

⭐ If you like this project, consider giving it a star!
