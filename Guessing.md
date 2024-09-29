# Guess That Number Game

```mermaid
flowchart TD;
  Start([Start])-->RandomNumber([Generate a number between 1-100]);
  RandomNumber-->PlayerInput([Get Player input]);
  
  PlayerInput--Correct-->CorrectGuess([Correct!]);
  PlayerInput--TooHigh-->WrongGuessHigh([Too High! Try Again]);
  PlayerInput--TooLow-->WrongGuessLow([Too Low! Try Again]);
  
  WrongGuessHigh-->PlayerInput
  WrongGuessLow-->PlayerInput
  CorrectGuess-->End([End])
```

The game begins with the system generating a random number between 1-100   The player must then guess a number between 1-100  
The game will then give feedback to the player based on the guess    
If guess is wrong, the player must try again until the correct number has been guessed    
Once the correct number has been guessed, the game will end.
