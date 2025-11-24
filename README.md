🐶 Virtual Pet Simulator (Python)
A simple, text-based command-line game where you adopt and care for a virtual pet. Keep your pet happy, fed, and clean by managing its statistics through an interactive menu.

📝 Description
This Python script simulates the experience of owning a pet. The program runs in a loop, allowing the user to perform various actions (like feeding or playing) which affect the pet's internal statistics. The pet's mood changes dynamically based on its current status.

🚀 How to Run
Prerequisites: Ensure you have Python installed on your computer.

Save the file: Save the code as pet_game.py.

Run the game: Open your terminal or command prompt and run:

Bash

python pet_game.py
🎮 Game Mechanics
Statistics
The pet starts with 50 points in every category. The goal is to keep these numbers high!

Hungry: Represents fullness. (Higher = Full, Lower = Starving)

Energy: Represents stamina.

Cleanliness: Hygiene level.

Happy: Happiness level.

Health: Physical wellbeing.

Actions
Each action affects the pet's stats differently:

Feed: (+20 Hunger, -10 Cleanliness)

Bath: (+30 Cleanliness, -10 Energy, +10 Happy)

Sleep: (+20 Energy, -20 Hunger)

Play: (-20 Energy, +30 Happy, -20 Hunger)

Bark: (-20 Energy, -10 Hunger)

Mood System
The pet will tell you how it feels based on its lowest stats:

Hungry: If hunger drops below 70.

Sleepy: If energy drops below 30.

Sick: If health drops below 50.

Sad: If happiness drops below 40.

Irritated: If cleanliness drops below 30.

📂 Code Structure
The project is structured into functional blocks for easy readability:

create_pet(): Initializes the pet dictionary with a name and default stats.

status_of_pet(pet): Displays the current statistics to the console.

mood_of_pet(pet): Checks stats and updates the 'mood' string.

feed_pet, bath_pet, sleep_pet, play_pet, bark_pet: Action functions that mathematically modify the pet's stats.

game_over(pet): Logic to check if the pet has died (stats <= 0).

main(): The primary game loop that handles user input and menu selection.

⚠️ Known Issues / To-Do
Game Over Logic: The game_over() function is defined but is not currently called inside the main while loop. The game currently continues indefinitely until the user selects "Quit."

Input Validation: The game currently expects number inputs (1-7). Non-numeric inputs may cause errors.

📜 License
This project is open-source and free to use or modify.
