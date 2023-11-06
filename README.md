# Land_of_Despair(first_game_created)
Land of Despair is a 2D game developed in C# using Visual Studio 2022 and the Monogame extension. This top-down shooter game challenges players to survive waves of zombies, collect valuable items, and achieve high scores as they progress through rounds.

The full PDF can be sent if requested, but here is some of the basic documentation that went into the game:
> ### Panning

Score based performance allows players to receive a score to improve on, allowing for competition, leading into increasing difficulty in levels to show off skill, to see how far you as a player can go. Collectables and enemies should allow for strategy and challenges to the player, allowing players navigate carefully, furthermore having an interface being user friendly, will make it easy for the player to understand and be able to focus on the gameplay. The deadline set to complete all stages of game development is 11 weeks.


> ### Game Design

My game design centres around surviving waves of zombies while gathering valuable items like gold, silver, and gems to accumulate points. You can also earn points by eliminating zombies. As the rounds progress, the number of zombies intensifies, making higher rounds more challenging to endure. This demands skill to reach higher levels. Losing a life occurs when a zombie hits you, and players start with 3 lives. Once all 3 lives are depleted, it's game over. 

**Key Features:**
- Top-down perspective gameplay
- Increasingly challenging rounds of zombies
- WASD keys for movement
- Mouse aiming for the space gun
- Scoring system based on zombie elimination and item collection
- Three lives per game


**The aim**
Is to see how long you can survive for, due to it being a round based game, meaning you can gain points and survive rounds to reach a high score.


**Scoring**

| Item      | Points Awarded |
|-----------|----------------|
| Gold      | 50             |
| Silver    | 25             |
| Gem       | 75             |
| Zombie    | 100            |


**Rounds**
(Let N = round number)

- Zombie health =50+100N
- Zombies spawn delay =10-((N-1))/2  
- Zombie count per round =2N+4
- Zombie movement speed =6+N/2


**Game algorithm (pseudo code)**

Start
If player presses the W key, the player moves forward.
If player presses the S key, the player moves backward.
If player presses the A key, the player moves to the left.
If player presses the D key, the player moves to the right.
If player presses the left mouse key, the player shoots bullets.
If the player walks into Gold, the player's score increases.
If all zombies are killed, the round increases, and zombies spawn.
If a zombie walks into the player, the player loses a life.
If the player loses all lives, the game over screen is displayed.
End


> ### Test plan that took place

**Functional Testing**
- Player Movement
- Player Health
- Zombie Spawning
- Zombie Movement
- Firing Weapon
- Wall collusion
- Round Completion
- Score Calculation
- Game Over

**Usability Testing**
- Controls and inputs
- Shooting Accuracy
- Collectable items are visible
- Round Progression
- User Interface Layout

**Stability and Performance**
- Multiple Zombies Spawning
- Bullet Count
- Game Responds
- Error Handling
- Memory Usage
- Loading Time
- Resource Utilization
- Long-Duration Gameplay


> ### Development

**Early gameplay** 

- Character Movement and shooting has been added
- The hazards (Enemies) will chase the player and make them lose a life 
- Points are rewarded when eliminating a zombie
- A round base has been added allow for hoards to spawn each round increasing in numbers and allowing for more of a challenge

**Finished gameplay**

Including all the early gameplay features as already stated.
- A Game Over screen has been added, showing the round survived to and the overall score achieved 
- Updated Player and Zombie textures which both changes depending on movement 
- Collectable points have been added, allow the player to increase their score by picking up the items.
- Background image added
- Timer has been added in the top right


> ### Review

I feel like I have a great foundation for an entertaining game but can be improved by adding power ups, adding the objective sprites, adding more weapons and a retry option on end screen, but considering it to be my first game and with a 11 week time frame, I think I did well.
