# Land of Despair (First Game Created)
Land of Despair is a 2D game developed in C# using Visual Studio 2022 and the Monogame extension. This top-down shooter game challenges players to survive waves of zombies, collect valuable items, and achieve high scores as they progress through rounds.

The full PDF can be sent if requested, but here is some of the basic documentation that went into the game:
> ### Panning

Score based performance allows players to receive a score to improve on, allowing for competition, leading into increasing difficulty in levels to show off skill, to see how far you as a player can go. Collectables and enemies should allow for strategy and challenges to the player, allowing players navigate carefully, furthermore having an interface being user friendly, will make it easy for the player to understand and be able to focus on the gameplay. The deadline set to complete all stages of game development is 11 weeks.


> ### Game Design

My game design centres around surviving waves of zombies while gathering valuable items like gold, silver, and gems to accumulate points. You can also earn points by eliminating zombies. As the rounds progress, the number of zombies intensifies, making higher rounds more challenging to endure. This demands skill to reach higher levels. Losing a life occurs when a zombie hits you, and players start with 3 lives. Once all 3 lives are depleted, it's game over. 

### Key Features:
- Top-down perspective gameplay
- Increasingly challenging rounds of zombies
- WASD keys for movement
- Mouse aiming for the space gun
- Scoring system based on zombie elimination and item collection
- Three lives per game
- The aim is to see how long you can survive, with round-based scoring.

### Playable Character Movement 
When any of the WASD keys are pressed, the character will change direction:

![Playable Character Walking](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/6287b3ed-c281-4460-ac44-f0ff93150b51)

### Zombie Movement
Depending on the direction the player is moving, will determine the zombies direction:

![Zombie Walking](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/faa5deeb-7fcf-4314-9b35-2b80f29033c2)

### Weapon

| Image                                                                                                                     | Item            | Contribute                         |
|---------------------------------------------------------------------------------------------------------------------------|-----------------|------------------------------------|
|![Energy Pistol](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/acb55a4b-689d-4f8a-97f0-8f89c0b37c0d)| Energy Pistol   | Used at range to eliminate zombies |               


### Scoring

| Image                                                                                                                       | Item   | Points Awarded |
|-----------------------------------------------------------------------------------------------------------------------------|--------|----------------|
| ![Gold](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/d6549b36-921d-4253-9078-c4cf36a56c5d)          | Gold   | 50             |               
| ![Silver](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/6882a6f9-124a-41f7-b425-72da191787c2)        | Silver | 25             |
| ![Gem](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/7638da05-ce74-42b2-97af-90d3160ba12e)           | Gem    | 75             |
| ![Zombie Walking](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/b0cf70a2-cd91-426c-911f-d46bae8a96bb)| Zombie | 100            |

### Extra Items

| Image                                                                                                                     | Item   | Effect |
|---------------------------------------------------------------------------------------------------------------------------|--------|--------|
|![Heart](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/423e6f22-0ca3-4df5-a389-6abce58154e4)        | Heart   | Extra life, which when picked up, will add another heart to the HUD bar             |               
|![Lighting Bolt](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/46155817-0955-4ada-b7b1-895deea30496)| Lightning Bolt | Speed up the character movement by x2              |

### HUD
An example of the lifes and score:

![HUB Example](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/528620d3-7c8b-4f9b-80aa-cfe89eb8b035)

These are health bars for players lives between 0 – 4 lives:

![0 Health](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/5a9552a5-db36-4da3-904f-3d936a302b8e)
![1 Health](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/33f7a873-5097-44d3-809c-8bc31987182e)
![2 Health](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/12208c00-a13c-4f43-a356-19e2151e3aa7)
![3 Health](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/40d3035e-4e18-4c3f-b28a-647734edd11e)
![4 Health](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/ad91af7d-714d-4e08-b7a7-c287ba236a6a)


### Map
I went with a basic cave map, that will allow sprites to easly stand out to the player:

![Map](https://github.com/CharlieWoodhouse/Land_of_Despair/assets/147112008/ac2f38b0-ddc2-4e28-9ed5-f6434810b289)


### Rounds
(This is subject to change when implemented into the game)

(Let N = round number)

**Zombie health =50+100N**

| Round      | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|------------|---|---|---|---|---|---|---|---|---|----|
| Health     |150|250|350|450|550|650|750|850|950|1050|

**Zombies spawn delay =10-((N-1))/2** (in seconds)

| Round      | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|------------|---|---|---|---|---|---|---|---|---|----|
|Spawn Delay |150|250|350|450|550|650|750|850|950|1050|

**Zombie count per round =2N+4**

| Round      | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|------------|---|---|---|---|---|---|---|---|---|----|
|Zombie Count| 6 | 8 | 10| 12| 14| 16| 18| 20| 22| 24 |

**Zombie movement speed =6+N/2**

| Round      | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8  | 9  | 10 |
|------------|---|---|---|---|---|---|---|----|----|----|
| Speed      |6.5|7.0|7.5|8.0|8.5|9.0|9.5|10.0|10.5|11.0|


### Game algorithm (pseudo code)
```python
Start

If player presses the W key
player moves forwards. 

If player presses the S key
Player moves backwards.

If player presses the A key 
Player moves to the Left.

If player presses the D key
Player moves to the Right. 

If player presses the Left mouse key
Player shoots bullets.

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
```

> ### Test plan

### Functional Testing

| Test ID | Test              | How I Tested                                     |
|---------|-------------------|--------------------------------------------------|
| 1       | Player Movement   | WASD all responsive and moves accurate           |
| 2       | Player Health     | Allow Zombie to hit player                       |
| 3       | Zombie Spawning   | Increase the round number                        |
| 4       | Zombie Movement   | Move the player around the screen                |
| 5       | Firing Weapon     | Clicking the left mouse button                   |
| 6       | Wall collusion    | Move the player to a wall                        |
| 7       | Round Completion  | Eliminate all zombies spawned                    |
| 8       | Score Calculation | Pick up Gold, Silver, Gems and eliminate zombies |
| 9       | Game Over         | Make the players health reach zero               |

### Usability Testing

| Test ID | Test                          | How I Tested                                            |
|---------|-------------------------------|---------------------------------------------------------|
| 1       | Controls and inputs           | Using WASD and Left mouse click                         |
| 2       | Shooting Accuracy             | Use Left mouse click to try and shoot zombies           |
| 3       | Collectable items are visible | Locating the collectable items                          |
| 4       | Round Progression             | Shooting zombies to go up the rounds                    |
| 5       | User Interface Layout         | Easy to glance as lives, score, and round on the screen |

### Stability and Performance

| Test ID | Test                      | How I Tested                               |
|---------|---------------------------|--------------------------------------------|
| 1       | Multiple Zombies Spawning | Spawning many zombies                      |
| 2       | Bullet Count              | Rapidly firing bullets                     |
| 3       | Game Responds             | Performing multiple actions simultaneously |
| 4       | Error Handling            | Including errors                           |
| 5       | Memory Usage              | Checking memory usage during gameplay      |
| 6       | Loading Time              | Launching the game                         |
| 7       | Resource Utilization      | Monitoring GPU and CPU usage while gaming  |
| 8       | Long-Duration Gameplay    | Playing the game for a long period         |

> ### Development

### Early gameplay

- Character Movement and shooting has been added
- Hazards (Enemies) will chase the player and make them lose a life 
- Points are rewarded when eliminating a zombie
- Round base has been added allow for hoards to spawn each round increasing in numbers and allowing for more of a challenge

### Finished gameplay

Including all the early gameplay features as already stated.
- Game Over screen has been added, showing the round survived to and the overall score achieved 
- Updated Player and Zombie textures which both changes depending on movement 
- Collectable points have been added, allow the player to increase their score by picking up the items.
- Background image added
- Timer has been added in the top right


> ### Review and Future Improvements

While Land of Despair is a great starting point, there are opportunities for future enhancements, such as adding power-ups, more objective sprites, additional weapons, and a retry option on the game over screen. Given the constraints of an 11-week development timeframe, I believe the game has achieved its goals effectively.
