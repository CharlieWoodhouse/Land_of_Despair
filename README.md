# Land_of_Despair(first_game_created)
This is a 2D game in C# using Visual Studio 2022 and the Monogame extension. It involves collecting items, avoiding hazards, managing lives, and progressively increasing difficulty as you advance through levels, aligning with specific scenario requirements and tasks that was assigned.

The full PDF can be sent if requested, but here is some of the basic documentation that went into the game:
> ### Panning

The aims and objectives needed to meet the target audience and expectations, such as gameplay that is engaging to the player, creating an enjoyable experience to keep people entertained and continue playing. Visual appearance, such as appealing graphics and animations to make it visually appealing to the target audience. Score based performance allows players to receive a score to improve on, allowing for competition, leading into increasing difficulty in levels to show off skill, to see how far you as a player can go. Collectables and enemies should allow for strategy and challenges to the player, allowing players navigate carefully, furthermore having an interface being user friendly, will make it easy for the player to understand and be able to focus on the gameplay. The deadline is 11 weeks complete all stages to create a fully functioning game.


> ### Game Designs

My game design centres around surviving waves of zombies while gathering valuable items like gold, silver, and gems to accumulate points. You can also earn points by eliminating zombies. As the rounds progress, the number of zombies intensifies, making higher rounds more challenging to endure. This demands skill to reach higher levels. Losing a life occurs when a zombie hits you, and players start with 3 lives. Once all 3 lives are depleted, it's game over. 

**Gameplay**
● The game will be a top-down perspective
● The game will involve rounds of zombies, which will increase in difficulty the higher the round gets.
● The player will be able to move around the map by using W, A, S, and D keys
● The player will be able to aim weapons (which will have unlimited ammo)
● Players will earn points by eliminating zombies and picking up treasure (gold, silver, and gems)    


**The aim**
Is to see how long you can survive for, due to it being a round based game, meaning you can gain points and survive rounds to reach a high score.


**Scoring**

Gold – 50 points will be awarded on pick up. 
Silver – 25 points will be awarded on pick up.
Gem – 75 points will be awarded on pick up. 
Zombie – 100 points will be awarded when eliminated.


**Rounds**
_Let N = round number_

Zombie health =50+100N
Zombies spawn delay =10-((N-1))/2  
Zombie count per round =2N+4
Zombie movement speed =6+N/2


**Game algorithm (pseudo code)**

Start

If player presses the W key
player moves forward. 

If player presses the S key
Player moves backwards.

If player presses the A key 
Player moves to the Left.

If player presses the D key
Player moves to the Right. 

If player presses the Left mouse key
Player shoots bullets 

If player walks into Gold
Player score gets increased by value set.

If player walks into Silver
Player score gets increased by value set.

If player walks into Gem 
Player score gets increased by value set.

If all zombies are killed
Round increases and zombie’s spawn.

If zombie walks into player 
Player loses life.

If player loses all the lives
End screen gets displayed. 

End


> ### Test plan created

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

●Character Movement and shooting has been added
●The hazards (Enemies) will chase the player and make them loose a life 
●Points are rewarded when eliminating a zombie
●A round base has been added allow for hoards to spawn each round increasing in numbers and allowing for more of a challenge

**Finished gameplay**

Including all the early gameplay features as already stated.
●A Game Over screen has been added, showing the round survived to and the overall score achieved 
●Updated Player and Zombie textures which both changes depending on movement 
●Collectable points have been added, allow the player to increase their score by picking up the items.
●Background image added
●Timer has been added in the top right


> ### Review

I feel like I have a great foundation for an entertaining game but can be improved by adding the power ups, adding the objective sprites, adding more weapons and a retry option on end screen, but considering it to be my first game and with a 11 week time frame, I think I did well.
