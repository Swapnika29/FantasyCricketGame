# FantasyCricketGame

This project is a Fantasy Cricket Game built with Python and PyQt5, where users can create and manage their dream cricket team, calculate scores, and visualize team performance. It uses an SQLite database to store team and player information.


## Features

Dream Team Creation: Allows users to select players from various categories (e.g., Batsmen, Bowlers, All-Rounders, Wicketkeepers) to form their fantasy team.

Points Management: Keeps track of available and used points for team creation.

Score Calculation: Computes team scores based on player performance in selected matches.

Database Integration: Uses an SQLite database (fantasy.db) for managing teams, players, and match data.

User Interface: Interactive UI created with PyQt5 for seamless user experience.


## Project Structure

The project consists of the following main components:

Files

1. dlgscore.py

    Contains the logic and UI implementation for the "Team Score" dialog.

    Displays scores for a selected team in a chosen match.

2. dream.py

    Implements the main application window.

    Provides functionalities for creating, opening, and saving teams.

    Includes points tracking, team validation, and player selection based on categories.

3. dream.ui:

    UI file for the main interface of the Fantasy Cricket Game.
   
    Designed using Qt Designer.

4. dlgscore.ui:

    UI file for the score calculation dialog.
   
    Designed using Qt Designer.

5. Database (fantasy.db):

    Stores teams, players, and their categories.
   
    Includes player performance statistics for score calculation.


## Dependencies


1. Python 3.7 or higher : Programming language used for this project.
2. PyQt5 : For creating the graphical user interface
3. SQLite3 :  For data storage and retrieval.


## How to Run the Project

1. Install Dependencies:

   a. Ensure you have Python 3.x installed.

   b. Install PyQt5 using pip:

          pip install PyQt5
     
   
2. Setup the Database:

   a. Create an SQLite database named fantasy.db.

   b. Populate it with the necessary tables and data.

3. Run the Application:

    Execute the main script (dream.py):

        python dream.py

4. Use the Application:


    a. Create a new team or open an existing one.

    b. Add players to the team, ensuring compliance with points and category limits.

    c. Save the team and calculate scores for matches.

   

## Usage Instructions

1. Create a New Team:

    a. Select "New Team" from the menu and enter a team name.

    b. Choose players from the available categories and add them to your team.

2. Save a Team:

    a. After forming a team, select "Save Team" to store it in the database.

3. Open an Existing Team:

    a. Select "Open Team" from the menu and choose an existing team from the database.

4. Calculate Team Score:

    a. Navigate to "Team Score" and select a team and match to calculate and view the team score.

  

## Rules and Constraints

1. Teams must consist of exactly 11 players.

2. Maximum players allowed per category:

    a. Batsmen: 5

    b. Bowlers: 5

    c. All-Rounders: 3

    d. Wicketkeepers: 1

3. Total points used must not exceed 1000.
