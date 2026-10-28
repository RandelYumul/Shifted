# Shifted

Shifted is a narrative-driven psychological mystery puzzle game built in Godot 4. The player follows Alex, who wakes up unable to remember the day before and slowly realizes that the world around them is changing. Rooms glitch, voices contradict each other, and the environment reacts to how well the player performs.

The game was developed for a hackathon in May 2026.

> **Content notice:** This game contains themes of memory distortion, identity fragmentation, and emotional trauma.

<!-- Add a screenshot: save it as docs/screenshot.png -->
![Shifted screenshot](sikap-tala/assets/pixel_art/pixel_folder/shifted.png)

---

## About the Game

Alex's morning starts like any other day: a phone call from Mom, a locked door, and a house that feels familiar. As the player explores, small details stop making sense. Familiar rooms return in distorted versions, the player is asked to make choices, and each puzzle or task affects what happens next.

The goal is to move through the house, solve each room's challenge, and uncover what really happened to Alex.

## Gameplay

- **Exploration:** Walk through the bedroom, hallway, kitchen, bathroom, and other locations, and interact with objects to find clues.
- **Puzzles:** Find hidden items, such as a key in a drawer, and solve a passcode lock to move forward.
- **Kitchen minigame:** Move a cup to catch falling sugar cubes while avoiding dark bubbles before the timer runs out. Each bubble caught removes 3 seconds.
- **Choices:** Pick between different options at key moments, which lead to different scenes.
- **Reactive world:** When the player fails a task, the environment shifts into a distorted "chaos state" with changing colors, flickering lights, and glitched rooms.
- **Multiple outcomes:** Success and failure lead to different scenes and endings.

## Controls

| Key | Action |
| --- | --- |
| A / D | Move left / right |
| E | Interact with objects |
| Enter / Space or mouse click | Continue dialogue and confirm |

## Technical Highlights

- **Engine:** Godot 4.6 (GDScript)
- **Dynamic environments:** CanvasModulate tweens and randomized lighting sequences create the visual distortion when the player fails.
- **Global audio:** A Global BGM Autoload (singleton) keeps background music playing smoothly between scenes.
- **Dialogue system:** A custom dialogue and textbox system handles conversations, inner thoughts, and choices.
- **Event-driven design:** Godot signals connect gameplay events to visual and audio effects.
- **Art and fonts:** Pixel art assets and the Pixelify Sans font.

---

## How to Run

1. Download and install [Godot 4.6](https://godotengine.org/download) (standard version).
2. Clone this repository:

   ```bash
   git clone https://github.com/RandelYumul/Shifted.git
   ```

3. Open Godot, click **Import**, and select the `sikap-tala/project.godot` file.
4. Press **F5** (or the Play button) to start the game.

## Project Structure

```
Shifted/
└── sikap-tala/
    ├── project.godot        Godot project file
    ├── game_backgrounds/    Main scenes and their scripts (rooms, menus, minigame)
    ├── Levels/              Bathroom and hallway scenes, player script
    ├── information/         Dialogue, textbox, puzzle, and global game state
    ├── character/           Player character scene
    ├── assets/              Pixel art, sprites, GIFs, and sound effects
    └── fonts/               Pixelify Sans font
```
