
# Perilous Python V1.0

### A Text-Based Adventure Game Built in Python

Welcome to Perilous Python, a beginner-friendly text-based RPG played entirely in the terminal.
Your goal is simple: explore the land, battle enemies, and ultimately defeat the Ancient Demon that has cursed the realm.

This project was developed as part of a software development learning module to demonstrate Object Oriented Programming, file handling,error management, and ethical programming practices.

## Purpose of the Application

Perilous Python was created to combin learning with creativity, allowing players to experience an RPG adventure while developers gain hands on practice with Python fundamentals.

The project demonstrates:

1. Object-Oriented Programming (OOP) through classes like `Character`, `Enemy`, and `Inventory`.
2. File Input/Output using JSON for saving and loading progress.
3. Error Handling & Logging through Python’s built-in `logging` library.
4. Randomisation via dice rolls to determine combat outcomes.

---

## Features of the Game

- Turn-Based Combat: Uses dice rolls to decide attack and defense results.
- Exploration: Move across a grid-style map from A1–D4, uncovering events and enemies.
- Inventory System: Collect and use items that affect health, attack, and defense.
- Save & Load Game: Store and reload progress using JSON.
- Boss Encounters: Includes both a main and optional boss.
- Error Logging: Combat errors are automatically logged for developer review.


## Setup & Installation

### Requirements

- Python: Version 3.12.3 or higher
- Code Editor: VS Code, PyCharm, Atom, or Sublime
- OS: Windows 10+, macOS 10.11+, or Ubuntu 16.04+

### Installation Steps

1. Download or clone this repository.
2. Open the project folder in your chosen code editor.
3. In your terminal, navigate to the folder containing `main.py`.
4. Run the program with:

   ``` python
   python3 main.py
   ```

## System Requirements
1. OS: Windows 10+, macOS 10.11+, choice of terminal (e.g. Ubuntu 16.04)
2. Processor: 1.6GHz dual-core or faster
3. Memory (RAM): 4GB
4. Storage: < 500MB
5. Display: laptop or computer display size is sufficient
6. GPU: Not required (text-based game)

## How to Play

The game provides interactive prompts throughout — simply follow on-screen text to explore, fight, and survive.

### Map & Movement

The map is a 4x4 grid labeled A1–D4, representing rows (A–D) and columns (1–4).
You move by typing "UP", "DOWN", "LEFT" or "RIGHT" in the terminal. 
for example, if you are at B2 and type UP in the terminal, your new location becomes A2.

![Diagram of A1-D4 grid](<sample_grid.png>)

### Combat

- Combat begins automatically when you enter certain zones.
- Battles are turn based, using dice rolls to decide hit or miss.

Example:

  ```
  You roll a 15 and hit the Skeleton for 10 damage!
  The Skeleton retaliates and hits you for 6 damage.
  ```
- Roll a 20 for a "Critical Hit", dealing double damage!

### Saving & Loading

- Type "save" or "save_game" to save progress anytime.
- Type "load" in the main menu to resume your saved game.
- Save files store stats, inventory, and events — enemies will respawn when you reload to maintain difficulty.

### Interactions

- Type "look" to observe your surroundings.
- Type "interact" to trigger events or collect items.

## Libraries Utilised
![Table of Libraries used](<libraries-table.png>)

## Example Code Documentation

### Function Example: "roll_dice()"

```python
def roll_dice(sides=6):
    """Rolls a dice and returns a random number between 1 and 'sides'."""
    return random.randint(1, sides)
```

- Purpose: Adds excitement and unpredictability to combat.
- Parameter: "sides" which is the number of dice sides (default = 6).
- Returns: A random integer from 1 to the chosen side count.
- Usage: Simulates dice rolls for hit/miss and critical hit outcomes.

### Class Example: "Player"

```python
class Player:
    """Represents the player character."""
    def __init__(self, name, health, attack, defense):
        self.name = name
        self.health = health
        self.attack = attack
        self.defense = defense
```

- Purpose: Defines player attributes for combat and progression.
- Used By: Game engine and combat system.
- Variables: Name, health, attack, and defense.
- Inheritance: None, this is a standalone class.

## Ethics & Licensing

- All libraries are open source under the Python Software Foundation License (PSFL).
- The project is distributed under the MIT License, allowing reuse with attribution.
* No personal data is collected and all save files remain local to the user’s computer.
* All code and text are original creations by the team.
* Accessibility: Works in all terminal environments and requires minimal system resources.
* Follows ethical coding principles therefore is transparent, open source, and respectful of user privacy.

## License (MIT)

This project is distributed under the MIT License. 

Permissions:
- Free use, copying, and modification allowed
- Commercial use permitted with attribution
- No warranty provided

For more details please view the MIT license overview: https://opensource.org/licenses/MIT 

## Error Handling

- This game included error handling to ensure smooth gameplay and easier debugging
- The logging library automatically creates a file named `Combat_errors.log`.
- If errors occur during gameplay, they’re recorded for review.
- Players can forward this log to the development team for bug reports.

## Feedback Log
- ADD HERE 

## Future Development

As this is a learning project, upcoming beginner-friendly improvements include:

- Expanded Map System: Add more grid locations or unlock new zones after defeating bosses.
- Simple Quest System: Introduce basic side quests that reward health potions or weapons.
- Visual Enhancements: Use ASCII art or color formatting (e.g., via the rich library) to make the game more immersive.
- Difficulty Settings: Include “easy,” “normal,” and “hard” modes to adjust enemy health and attack.

## References

1. Python Software Foundation License (PSFL): [https://docs.python.org/3/license.html](https://docs.python.org/3/license.html)
2. MIT License Overview: [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT)
3. W3C Accessibility Principles: [https://www.w3.org/WAI/fundamentals/accessibility-principles/](https://www.w3.org/WAI/fundamentals/accessibility-principles/)


