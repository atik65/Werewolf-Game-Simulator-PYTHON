# Reflection Section

## Question 1: Which part was the hardest?

The hardest part for me was figuring out the game-ending condition. At first, I did not realize that Werewolves win when their number equals or exceeds the Villagers. I kept checking if all villagers were dead, but that is not the same thing. I had to read the assignment requirements carefully a few times. Once I understood the rule, writing the `check_winner()` method was straightforward.

## Question 2: What bug/problem did you face?

I ran into a problem where the game would crash during the night phase if no werewolves were alive. My code tried to pick a random villager to attack, but it also assumed there was always a werewolf making the attack. I fixed this by adding a check at the start of the `night_phase()` method. Now if there are no alive werewolves, the night phase just prints a message and returns safely.

## Question 3: What did you learn from this assignment?

This assignment taught me how to use classes in Python for a real project. Before this, I only wrote small programs without classes. I learned how to separate different parts of a program into methods. I also learned about file handling — reading from `players.txt` and writing results to `game_result.txt`. The random module was fun to use for picking targets and suspects. Overall, I now feel more comfortable with object-oriented programming.

## Question 4: What would you improve later?

If I had more time, I would add more roles to the game, like a Doctor who can save one person each night or a Seer who can check someone's role. I would also make the game interactive so the user can type commands instead of just watching the simulation run. Another improvement would be adding a graphical interface using a library like `tkinter`. I think these additions would make the project more interesting and fun to play.
