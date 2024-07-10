
# Magical Arena

Welcome to the **Magical Arena** game! This project simulates a turn-based battle between two players in a magical arena. Players take turns attacking each other until one player's health reaches zero.

## Overview

In **Magical Arena**, each player has three attributes:
- **Health**: Determines how much damage the player can take before being defeated.
- **Strength**: Used to calculate the amount of damage blocked by the player.
- **Attack**: Determines the damage dealt by the player during an attack.

Players attack in turns, rolling dice to determine the attack and defense outcomes. The game continues until one player's health drops to zero.

## Requirements

To run the code, you need:
- **Java Development Kit (JDK) 11 or higher**: Ensure you have the JDK installed on your system.

## How to Compile and Run the Code

Follow these steps to set up and run the game:

1. **Unzip the Folder**:
   Extract the contents of the `MagicalArena.zip` file to your desired location.

2. **Open Terminal**:
   Navigate to the folder where the `src` and `test` directories are located.

3. **Compile the Code**:
   Run the following command to compile the Java source files:
   ```sh
   javac -d bin src/*.java test/*.java
   ```

4. **Run the Main Class**:
   To start the game, execute:
   ```sh
   java -cp bin MagicalArena
   ```

5. **Run the Test Class**:
   To execute the unit tests, run:
   ```sh
   java -cp bin MagicalArenaTest
   ```

## Example

### Game Input:

```
Enter attributes for Player A (health, strength, attack): 
50
5
10
Enter attributes for Player B (health, strength, attack): 
100
10
5
```

### Game Output:

```
Player A: Health: 50, Strength: 5, Attack: 10
Player B: Health: 100, Strength: 10, Attack: 5

Attacker rolls 5, Defender rolls 4
Attack damage: 50, Defense strength: 40
Defender health reduced by 10 to 90

Attacker rolls 5, Defender rolls 2
Attack damage: 25, Defense strength: 10
Defender health reduced by 15 to 75

Attacker rolls 2, Defender rolls 3
Attack damage: 20, Defense strength: 30
Defender health reduced by 0 to 75

...

Attacker rolls 4, Defender rolls 1
Attack damage: 20, Defense strength: 5
Defender health reduced by 15 to -10

Player B wins!
```

### Test Output:

```
Running testPlayerInitialization...
testPlayerInitialization passed

Running testPlayerIsAlive...
testPlayerIsAlive passed

Running testRollDie...
testRollDie passed

Running testFight...
Attacker rolls 4, Defender rolls 4
Attack damage: 40, Defense strength: 20
Defender health reduced by 20 to 30

testFight passed
```

## Author

**Vishal Shyam Dasani**

Code is added with comprehensive comments for easy explanation. In case of any doubts, contact [vishaldasani1999@gmail.com](mailto:vishaldasani1999@gmail.com).

## Code Files

- `src/Player.java`: Contains the `Player` class definition.
- `src/MagicalArena.java`: Contains the main logic for the game.
- `test/MagicalArenaTest.java`: Contains the unit tests for the game.

