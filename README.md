# Hangman Game

## Project Description

Hangman is an interactive word-guessing game developed using **HTML,
CSS, and JavaScript**. The player selects a category and difficulty
level, reads a clue, and guesses the hidden word letter by letter before
the available attempts run out.

The project is designed as a browser-based game and does not require a
separate backend or database.

## Features

-   Simple and responsive game interface
-   18 different word categories
-   3 difficulty levels: Easy, Medium, and Hard
-   50 levels for each category and difficulty
-   Total of **2700 levels**
-   Clues for every hidden word
-   Some letters are revealed automatically at the beginning of a level
-   Limited hints
-   Score system with bonuses and penalties
-   Hangman drawing updates after wrong guesses
-   On-screen alphabet keyboard
-   Supports typing guesses using a physical keyboard
-   Completed levels unlock the next level
-   Completed levels can be replayed
-   Progress and scores are saved in the browser using `localStorage`
-   Settings page to view progress and reset all saved progress
-   Mobile-friendly responsive design

## Categories

The game includes these 18 categories:

1.  Fruits
2.  Animals
3.  Countries
4.  Programming
5.  General Knowledge
6.  Movies
7.  Sports
8.  Food
9.  Vehicles
10. Cities
11. Science
12. Education
13. Music
14. Technology
15. History
16. Nature
17. Games
18. Books

Each category contains Easy, Medium, and Hard word banks.

## Difficulty Levels

  Difficulty     Attempts   Hints   Base Points
  ------------ ---------- ------- -------------
  Easy                  8       3           100
  Medium                6       2           200
  Hard                  5       1           300

-   **Easy:** Short and common words with more attempts and hints.
-   **Medium:** Longer vocabulary with fewer attempts and hints.
-   **Hard:** More difficult vocabulary with fewer attempts and higher
    base points.

Each difficulty contains 50 levels per category.

## Scoring System

The score for a completed level is calculated using:

-   Base score according to difficulty
-   Points for correct guesses
-   Penalty for wrong guesses
-   Hint penalty
-   Level completion bonus
-   Bonus for remaining attempts
-   Speed bonus
-   Extra no-hint bonus

Each hint costs **25 points**.

The score is never allowed to become negative.

## How to Play

1.  Open the HTML file in a web browser.
2.  Select **Play Game**.
3.  Choose a category.
4.  Select Easy, Medium, or Hard.
5.  Choose the available level.
6.  Read the clue.
7.  Guess letters using the on-screen keyboard or physical keyboard.
8.  Correct letters are revealed in the word.
9.  Wrong guesses reduce the remaining attempts and add a part to the
    Hangman drawing.
10. Reveal the complete word before all attempts are used.
11. Completing a level unlocks the next level.
12. Use hints when needed, keeping in mind that each hint costs points.

## Game Progress

The game saves progress on the same device using the browser's
`localStorage`.

The saved information includes:

-   Completed levels
-   Score for each category and difficulty
-   Overall completed-level count
-   Total score

The player can close the browser and return later without losing saved
progress.

The **Settings** page also provides an option to reset all progress.

## Technologies Used

-   **HTML5** -- Structure of the game
-   **CSS3** -- Layout, styling, animations, responsive design
-   **JavaScript** -- Game logic, level management, scoring, hints,
    keyboard controls, and progress storage
-   **Browser Local Storage** -- Saving game progress
-   **SVG** -- Hangman drawing and game icon

## Project Structure

This project is implemented as a single HTML file:

``` text
Hangman Project/
└── hangman (3).html
```

The HTML file contains:

-   HTML interface
-   CSS styling
-   JavaScript game logic
-   Category and word data
-   Difficulty configuration
-   Level generation
-   Scoring system
-   Progress storage

## How to Run

No installation is required.

### Method 1: Directly in a Browser

1.  Keep `hangman (3).html` in a folder.
2.  Double-click the HTML file.
3.  It will open in your default web browser.
4.  Click **Play Game** to start.

### Method 2: Using VS Code

1.  Open the project folder in Visual Studio Code.
2.  Open `hangman (3).html`.
3.  Open the file in a browser.
4.  If using the Live Server extension, right-click the HTML file and
    select **Open with Live Server**.

## Level Generation

The game creates 50 levels for every category and difficulty. The word
banks are shuffled using a seeded randomization method so that the level
arrangement is deterministic for a particular category and difficulty.

This allows the game to create multiple levels from the available word
bank without requiring separate hard-coded level definitions.

## User Interface

The game contains the following main screens:

-   **Home** -- Start the game, view instructions, open settings, and
    see overall progress.
-   **Categories** -- Select a word category.
-   **Difficulty** -- Select Easy, Medium, or Hard.
-   **Levels** -- View completed, current, and locked levels.
-   **Game** -- Guess the hidden word and earn points.
-   **How to Play** -- Displays game instructions.
-   **Settings** -- View saved progress and reset the game.

## Future Enhancements

Possible improvements include:

-   Add more word categories
-   Add sound effects and background music
-   Add a leaderboard
-   Add player profiles
-   Add more word banks
-   Add multiplayer mode
-   Add a dark/light theme switch
-   Add downloadable progress or cloud saving
-   Add a timer for individual levels

## Conclusion

This Hangman project provides an interactive and responsive
word-guessing experience using only front-end web technologies. Its
category system, multiple difficulty levels, scoring, hints, level
progression, and local progress storage make it suitable as a college
web development project.
