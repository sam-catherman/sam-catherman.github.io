# Guessing Game Flowchart

```mermaid
flowchart TD
    Start([Start]) --> Input[("User inputs a guess")]
    Input --> Check[("Check if guess is correct")]
    Check -->|Correct| End([End - You guessed it!])
    Check -->|Too High| Hint1[("Provide hint: Guess lower")]
    Check -->|Too Low| Hint2[("Provide hint: Guess higher")]
    Hint1 --> Input
    Hint2 --> Input
## Process Description
-**Start**: The game begins.
-**User inputs a guess**: The player inputs their guess for the number.
-**Check if guess is correct**: The game compares the user's guess to the correct number.
-**If Correct**: If the guess is correct, the game ends and displays a success message.
-**If Too High**: If the guess is too high, the game provides a hint to "Guess lower" and prompts the user to enter a new guess.
-**If Too Low**: If the guess is too low, the game provides a hint to "Guess higher" and prompts the user to enter a new guess.
-**Repeat**: Steps 2-6 are repeated until the user guesses the correct number.
-**End**: Once the user guesses correctly, the game concludes.
