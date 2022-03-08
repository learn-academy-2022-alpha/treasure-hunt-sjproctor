# React Treasure Hunt Game

### Remember:
- Pseudocode!!
- Ask clarifying questions

### User Stories
- As a user, I can see a page with a 3 by 3 grid board game with a question mark in each square. (done)
  - Got one square to render
  - Mapped the array in state and returned the Square component call to get nine squares
  - Used flex properties to create the board game
  - Passed the value of the map into the Square component
  - Added styling for a pleasant user experience
- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array. (done)
  - Added an onClick to each square
  - Attached a method to the onClick
  - Pass the index of the array and reference the index as props
  - Created a method in App.js
  - Passed the method to Square and referenced it as props
  - Added a parameter to alert the index
- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji. (done)
  - Destructure board out of state
  - Used the index parameter to reassign the square that is clicked
  - setState with the updated array
- As a user, if I select the winning square the question mark will become a treasure emoji. (done)
  - Add treasureLocation to state
  - Add a componentDidMount that will create a random number for the treasureLocation
  - Set the random number to state
  - Add a conditional to the handleGamePlay method to manage the two different outcomes
- As a user, if I select the losing square the question mark will become a bomb emoji.
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at 5 and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).
- As a user, I can click on a “Play Again” button that will restart the game.
