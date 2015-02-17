#Introduction

The purpose of this lab was to modify an open source game engine to provide the user with statistics on their performance within the game. This modification would then be used to design an experiment to determine the effectiveness of the controllers we constructed in the previous 2 labs.

#Design Methodology

The statistics I felt were the most important to track were the time the user spent alive, the hits to shots ratio (commonlly referred to simply as accuracy), and the kill:death ratio. These are imporant because the first metric measures how good a player is at the movement aspect of the game by determining their ability to dodge shots, the second metric measures the aiming of the player, and KD ratio measures overall skill, taking both into account. 

I also decided to measure the ratio of successful damage to opponents vs. damage attempts because the necessary code was already mostly in place. This metric can be coupled with the standard accuracy to see what types of weapons may be more or less accurate with the controller.

I measure most of these metrics whenever the player respawns so that the player's performance can be tracked throughout the course of a single 10 minute game. These are stored in a simple txt file which I then manually converted to a CSV. The one metric that had to be handled seperately was total shots. Since this is handled client side, I created a new file which would simply put a mark on a text file everytime the player shot. I sent a new line character when the player respawned to kep track of which set of marks corresponded to which life.

#Testing Methodology

For the testing I chose to use 5 level 90 bots on the map I felt most farmiliar with. I chose level 90 bots because it would give consistant difficulty between tests and I felt level 90 was challanging but still relitively easy to succeed in. Furthermore, from brief perliminary tests, I found that it would be fairly easy to not die if I focused purely on movement and health pick ups. At higher difficulty levels, I found that I would occasionally die in a manner I could not have predicted beforehand.

I chose to test 3 "controllers", the one I built in labs 1 and 2, the sample controller built by Professor Spjut, and a standard keyboard and mouse as a benchmark. I first played one 10 minute game with each controller, followed by 3 more games this time in the reverse order. this should make it clear if the change in performance is due to player learning or if the controllers are really affecting the performance.

#Results and Discussion

#Conclusions
