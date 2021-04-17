# Simulating results based on xG 

Posting sums of xG over the game is a common practice on Twiiter. And it's wrong. Probabilities are weird and just summing them is over simplifying it.

I have put together an xG based inforgraphic of a game. This is created after simulating the sequence of shots and the xG of each many many times over, recording each shot as a goal or not based on the simulation, and keeping count of how many times we saw each of the scenarios depicted here.

![](./ManchesterCity_Leeds_14740.png)

There is a lot happening here so I'm going to quickly deconstruct it:
- Row 1, column 1: The probabilities of various goal difference values at any point in time during the game, based on the shots upto that point. The probability bands are vertically sorted in order of goal difference such that the highest goal difference towards Manchester City winning is always at the bottom and the highest goal difference towards Leeds winning is always at the top. The band with the dark outline tracks the band for the actual eventual goal difference.
- 1,2: More information about the probability distribution of various goal difference values at the end of the game after all the shots have been taken.
- 1,3: Spltting each goal difference value further into the probabilities of the individual scorelines which could lead to the goal difference.
- 1,4: The probabilities of various goal difference values possible at the end of the game, based the actual events during the game until time x, i.e. goal or no goal for each of the shot, and the sequence of shots remaining after time x.
- 2,1: Similar to 1,1 except each probability band is a particular score and the vertical sorting is such that the lowest probability score line is at the bottom, and the highest probabilty scoreline is at the top.
- 2,2: Similar to 1,2 except each probability band is a particular score and the vertical sorting is such that the lowest probability score line is at the bottom, and the highest probabilty scoreline is at the top.
- 2,3: Summary of the simulations
- 2,4: Similar to 1,4 except each probability band is a particular score and the vertical sorting is such that the lowest probability score line is at the bottom, and the highest probabilty scoreline is at the top.
- 3,1: Each shot and the xG of each shot along the duration of the game
- 3,2: The overall sum of xG and count of shots, which is not enough information about the game. This is kept here for the viewer to appreciate all the information that this is not able to capture.
- 3,4: Each shot and the xG of each shot along the duration of the game

Beyond what is mentioned in the summary in the infographic already, other observations include:
- By the time Leeds scored their first goal, Manchester City were ahead by at least one goal in around 60% of the simulations. You can see this in 1,1.
- City were more likely to win 1-0, 2-0, or 3-0 than any draw.  You can see this in 2,2.
- The final 1-2 scoreline was pretty unlikely until Leeds scored their first goal. After City's goal, the remaining shots gave both teams an almost equal chance of winning 2-1, with around a 75% probability of the game ending in a draw.  You can see this in 1,4 and 2,4.
- Before City scored their goal, Leeds had more than a 50% chance of winning by one goal based on the shots that were yet to happen. Most of it came from the possibility of a 0-1 win.  You can see this in 1,4.
- City's first goal came at a point where the probability of them winning by at least one goal was barely 10%. All their shot attempts after that goal were only enough to increase their chance of winning to a little over 25%.  You can see this in 1,4.