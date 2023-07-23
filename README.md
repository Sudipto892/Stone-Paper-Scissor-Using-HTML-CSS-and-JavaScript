# Stone-Paper-Scissor-Using-HTML-CSS-and-JavaScript
The stone, paper, and scissors game is a simple and enjoyable game in which both players must create a stone, paper, or scissors. It can only have two outcomes: a draw or a win for one player and a loss for the other. We created a JavaScript game in which a player competes against the machine. There will be a total of 5 moves. The player must select one of the three options: stone, paper, or scissors. The computer will select a random alternative, and the winner will receive one point each time. The ultimate result will be presented on the screen after 5 moves, along with a button to restart the game.  

# Steps for creating Rock-Paper-Scissors Game
To create a Stone-Paper-Scissors Game using HTML, CSS, and vanilla JavaScript, follow the given steps line by line:-

Create a folder. You can name this folder whatever you want, and inside this folder, create the mentioned files.
Create an index.html file. The file name must be index and its extension .html
Create a style.css file. The file name must be style and its extension .css
Create a script.js file. The file name must be script and its extension .js

# The HTML Layout:
HTML gives the basic structure of the game. styles.css file is linked in the head tag which will be used for styling the HTML.
A div with the class title is used to display the title on the screen.
A div with a class score contains two more div which will display the score of the player and computer.
Div with the class move just displays a text and div with class movesleft will show the number of moves left before the game ends.
A div with a class option contains three button stone, paper, and scissors which the user can use to give the input.
A div with the class result will display the result of every move and the final result after 10 moves and the button with class reload will allow reloading the game.

# CSS Styling:
The CSS stylesheet is for a simple game interface with the following features:-
Universal styles for the entire document.
Game container to center content vertically and horizontally.
Styling for the game title and score display.
Styling for game buttons representing player moves.
Responsive design for smaller screens.

# The logic using JavaScript:
The main logic of the game is created by using JavaScript. We will be performing DOM manipulation so basic knowledge of JavaScript is enough to build the game.

Follow steps ->

Create a function game() that will contain all the logic of the game.
Inside the function declare three variables playerScore, computerScore, moves which will keep the record of the player’s score, computer’s score, and moves completed respectively.
Create a function playGame() and inside the function use DOM manipulation to get hold of all the three buttons we created in HTML for player input. Create an array playerOptions which will contain all three buttons as its elements. Similarly, create an array for computer options.
Use forEach() loop on playerOptions so that we can add an event listener on all buttons with a single piece of code. Inside the loop increment moves counter by 1 display moves left on the screen by subtracting moves from 5. Generate a random value for the computer option and compare it with the player’s input.
Create a function winner() which will receive two arguments one the player’s input and the other the computer’s option  The function will decide who wins the point among the player and computer.
Create a function gameOver() which will display the final result with reload button. The function will be called when moves will become equals to 5.
Call the playGame() function inside the game() function.
Now call the game() function at the end of the file.
