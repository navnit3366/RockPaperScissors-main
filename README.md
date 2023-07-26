# RockPaperScissors Game
### Description
A simple beginner level rock paper scissors game using Python.

### Tools and Languages:
<img align="left" alt="Python" width="26px" src="python.png" />
<img align="left" alt="pip" width="26px" height="34px" src="pip.png" />
<img align="left" alt="VS Code" width="26px" src="vscode.png" />
<br>

### Installing Libraries
```cmd
pip install os
pip install re
pip install random
```
-> Mostly probably you should already have OS, random and re libraries installed as it comes with python distribution.

### Steps to follow
-Install the given libraries<br>
-Download the code from the given github repository<br>
-Run the code
-Enjoy the game<br>

### Breaking the code
Importing Libraries
```python
import random
import os
import re
```
Game Logic
```python
os.system('cls' if os.name=='nt' else 'clear')
while (1 < 2):
    print ("\n")
    print ("Rock, Paper, Scissors - Shoot!")
    userChoice = input("Choose your weapon [R]ock], [P]aper, or [S]cissors: ")
    if not re.match("[SsRrPp]", userChoice):
        print ("Please choose a letter:")
        print ("[R]ock, [S]cissors or [P]aper.")
        continue
    print ("You chose: " + userChoice)
    choices = ['R', 'P', 'S']
    opponenetChoice = random.choice(choices)
    print ("I chose: " + opponenetChoice)
    if opponenetChoice == str.upper(userChoice):
        print ("Tie! ")
    #if opponenetChoice == str("R") and str.upper(userChoice) == "P"
    elif opponenetChoice == 'R' and userChoice.upper() == 'S':      
        print ("Scissors beats rock, I win! ")
        continue
    elif opponenetChoice == 'S' and userChoice.upper() == 'P':      
        print ("Scissors beats paper! I win! ")
        continue
    elif opponenetChoice == 'P' and userChoice.upper() == 'R':      
        print ("Paper beat rock, I win! ")
        continue
    else:       
        print ("You win!")
```

### Developed by:
<a href="https://github.com/ankush0939">Ankush Mishra</a>
