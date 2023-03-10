
#   PROTEIN-ROCKS!


## [See the Game](https://dagmaro.github.io/Protein-rocks-/)

# Description

PROTEIN-ROCKS! is a game where the player (Dwayne Johnson) has to move horizontally and vertically to pick up his protein shake meanwhile pizzas will start falling down from the top of the screen and some french toast will appear from the right side of the screen. In both cases our player has to dodge them.
Pizzas will decrease your health life because are more unhealth and french toast will decrease your score! but if your score hits 0, the french toast will start decreasing your health too!

# Main Functionalities

- Our player moves horizontally and vertically
- Our player can bend himself and return to his original height
- Pizzas appear randomly from the top of the screen
- French toast appear randomly from the right side of the screen
- If a pizza catch you X time the game ends.

# Backlog Functionalities

- Ability to increase the difficulty
- Ability to have a "main enemy" so if we achieve X score, every oher enemy would disappear and it would appear one big enemy so you have to start shooting him to pass to another level.
- Ability to move the screen vertically so our player can jump on some platforms picking his protein meanwhile it would appear our enemies randomly and if the screen below catches you, the game ends.
- Improve the player movement, make it more smoothly


# Proyect Structure

- List here the JS files you think you might need. 
- One main.js to manage DOM elements, one for Game class and one for each other class.
- Recommended: Inside each file you can list the functions, clases, properties and methods you will need.

Example:

## script.js

- startGame()
- endGame()
- moveRight()
- moveLeft()
- bend()
- moveUp()
- standUp()
- moveDown()

## game.js

- Game () {
    this.background;
    this.dwayne = new Dwayne();
    this.pizza = new Pizza();
    this.protein = new Protein();
    this.frenchToast = new Toast();
    this.pizzaArr;
    this.proteinArr;
    this.frenchToastArr;
    this.score;
    this.time;
    this.gameOn;
    this.health;
    this.lessHealth;
    this.mySound = new Audio (this game has 4 different sounds for our collisions with the objects and one for the END GAME)
}
- drawBackground() {}
- proteinAppears() {}
- pizzaAppears() {}
- frenchToastAppears() {}
- drawScore() {}
- drawHealth() {}
- collisionProteinWithDwayne() {}
- collisionPizzaWithDwayne() {}
- collisionToastWithDwayne() {}
- collisionDwayneWithSideWalls() {}
- collisionDwayneWithUpAndDownWalls() {}
- gameOver() {}
- clearCanvas() {}
- gameLoop () {}


## Dwayne.js 

- Dwayne () {
    this.x;
    this.y;
    this.w;
    this.h;
    this.jumpSpeed;
    this.speedX;
    this.speedY; (we have to speeds in case one day we would want to change to jump instead moving up)
    this.img;
    this.gravity;
}
- drawDwayne () {}
- rightMovement() {}
- leftMovement() {}
- downMovement() {}
- upMovement() {}
- bendMovement() {}
- standUpMoevement() {}

## Pizza.js 

- Pizza() {
    this.h;
    this.w;
    this.x;
    this.y;
    this.speed;
    this.image;
}
- drawPizza() {}
- charactersMove() {}

## frenchToast.js 

- Toast() {
    this.h;
    this.w;
    this.x;
    this.y;
    this.speed;
    this.image;
}
- drawToast() {}
- charactersMove() {}

## protein.js 

- Protein() {
    this.w;
    this.h;
    this.x;
    this.y;
    this.speed;
    this.image;
    this.collected;
}
- drawProtein() {}

# States and Transitions

- splachScreen
- gameScreen
-  gameOverScreen

# Extra Links (The links can be added later when available)

### Trello
[Link](www.your-url-here.com)

### Slides
[Link](https://www.canva.com/design/DAFZguTlMR8/Mb8azqdtiu-JPt59cCJZPg/view?utm_content=DAFZguTlMR8&utm_campaign=designshare&utm_medium=link&utm_source=homepage_design_menu)