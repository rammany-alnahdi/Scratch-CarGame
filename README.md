# Scratch Learning Project | An Intro to Game Programming

<p align="center">
  <img src="movement.png" width="48%" alt="Movement Code" />
  <img src="animation.png" width="48%" alt="Animation Code" />
  <img src="buildcode.png" width="48%" alt="buildCode" />
  <img src="gamemap.png" width="48%" alt="Game map" />
</p>

Welcome to your first real coding lesson! This project is a simple, fully playable 2D game built in Scratch. It was designed from the ground up to teach the fundamental building blocks of computer science in a fun, visual, and interactive way.

By building this game, we are learning the exact same concepts that professional software engineers use to build mobile apps, websites, and 3D video games.

## 📚 Core Coding Concepts Learned

This game is broken down into four major "Lessons." Here is what the code behind the scenes is actually doing:

### Lesson 1: The X/Y Coordinate Grid (Player Movement)
To move our character, we have to understand the mathematical grid. 
* **The Code:** We use `When [Key] Pressed` event blocks. 
* **The Concept:** The screen is a giant invisible graph. Pressing the **Up Arrow** increases the `Y` value (moving up), and the **Down Arrow** decreases `Y`. The **Right Arrow** increases the `X` value, and the **Left Arrow** decreases `X`. 
* **Teacher's Challenge:** Try changing the `change x by 10` block to `change x by 50`. What happens to the character? *(Answer: They move much faster!)*

### Lesson 2: The `Forever` Loop (Animation)
How do we make the character look like they are actually flying or walking instead of just sliding across the screen?
* **The Code:** We put a `Next Costume` block inside a `Forever` loop, with a `Wait 0.2 secs` delay.
* **The Concept:** This is called a **Loop**. Instead of writing the code 1,000 times to flap the wings, the loop tells the computer to continuously swap pictures (costumes) over and over until the game ends. The 0.2-second delay is our "Frame Rate"—it stops the wings from flapping too fast!

### Lesson 3: Variables (Keeping Score)
A game needs a way to remember how well you are doing. We do this using computer memory.
* **The Code:** `Set [Score] to 0` at the start, then `change [Score] by 1` every second.
* **The Concept:** This is a **Variable**. Think of a variable as a digital box with a name on it. We named our box "Score". Every second, the computer opens the box, takes out the old number, adds 1 to it, and puts the new number back in the box. 

### Lesson 4: Event Broadcasting (The "Game Over" Screen)
When our character hits an obstacle, how does the background know it is time to change to the "Lose" screen?
* **The Code:** `When I receive [lose]` -> `Switch backdrop to [lose]` -> `Stop [all]`.
* **The Concept:** Sprites in Scratch need a way to talk to each other. This is called **Event Messaging**. When the player hits a bad guy, the player sprite shouts a secret message ("lose!") across the whole program. The background hears this message and instantly changes the picture, and the game stops all running loops.

---

## 🎮 How to Play

1. Click the **Green Flag** to start the game.
2. Use the **Arrow Keys** (⬆️ ⬇️ ⬅️ ➡️) on your keyboard to navigate the character.
3. Dodge the falling obstacles!
4. Survive as long as you can to increase your **Score**.
5. If you touch an obstacle, it's Game Over! Press the Green Flag to try again.

## 🛠️ Homework for the Student

Want to make the game your own? Open the code and try changing these things:
* **Make it harder:** Find the `Wait 1 secs` block in the obstacle code and change it to `0.5 secs`. Now the enemies will spawn twice as fast!
* **Change the character:** Go to the "Costumes" tab and draw a hat on your character, or pick a completely new animal to play as.
