Rock Paper Scissors Project
---------------------------
-The game is currently working with two functions
-Below is algorithm and working ideas for the game
-Ideas to work on:
  -continuing the game until the best out of 5 has been won
  -limiting the game to only the console
    -at the moment, the game runs from prompt and alert functions as well as console log
    -pushing the rules of win and lose rules to a helper function to make the playRound function shorter and easier to read
    

PROBLEM
-Create a console game that the user plays against a computer
-The computer turn will be completely randomized
  -write a function that handles the computers turn
-Player selection should be case sensitve
-Create a game function to have the game play five rounds
  -prompt the user for their selection at the beginning of each round
  -keep score at the end of each round

DATA TYPES
-strings
  -user input and computer turn input
    -"Rock", "paper", or "scissors"
  -user prompt for input of three selections
  -string that returns whether the play wins or loses
-integers
  -used to count the number of games played
  -used to count the number of wins and losses

ALOGRITHM
-create a variable named possibleOptions set to the array ["rock", "paper", "scissors]
-create a variable named computerSelection set to the random selection of possibleOptions
-Create a variable named playerSelection set to the prompt return asking the user for 'rock, paper, or scissors'
-Write a function named playRound that takes two parameters of playerSelection and computerSelection
  -call the variables playerSelection and computerSelection
  -if playerSelection and computerSelection are equal
    -return "it is a tie"
  -if playerSelection = "rock" and computerSelection = "scissors"
    -increment player score
    -return "you win"
  -else if playerSelection = "paper" and computerSelection = "rock"
    -increment player score
    -return "you win"
  -else if playerSelection = "scissors" and computerSelection = "paper"
    -increment playerScore
    -return "you win"

  -else
    -increment computer score
    -return "you lose"
GAME FUNCTION
  -create a variable named computerScore set to 0
  -create a variable named playerScore set to 0
  -create a function named game
    -create a for loop that counts up to 5 for 5 total games
    -inside of the loop
      -set the computerSelection equal to the computerPlay function
      -create variable named playerSection set to the return of the prompt "please choose: rock, paper, or scissors"
        -call the lowercase function on this variable
      -call the playRound function with the arguments playerSelection and computerSelection
    -if playerScore is greater than computerScore
      -console log "You win: playerScore and computerScore"
    -if playerScore is less than computerScore
      -console log "You lose: playerScore and computerScore"
    -else
      -console log "It is a tie! Playerscore and computerscore