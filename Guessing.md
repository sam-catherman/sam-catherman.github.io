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

# Process
