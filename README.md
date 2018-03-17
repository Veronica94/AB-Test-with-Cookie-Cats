# AB-Test-with-Cookie-Cats

This is a AB test project from *datacamp*. 

## Project Objective
The project aims to find out if the retention rate for a puzzle game, **Cookie Cats**, will be higher when the gate (i.e. force users to stop for a non-trivial time or make in-app purchase) is moved to level 40 as compare to level 30.

![Alt text](cc_gates.png?raw=true "Title")

## Dataset Overview
In the dataset, we have the following attributes:

- userid
- version: AB groups. Our control is gate_30 and treatment is gate_40
- sum_gamerounds: total number of game rounds played during the first 14 days after install
- retention_1: 1 if the player come back and play **1 day** after installing, 0 otherwise
- retention_7: 1 if the player come back and play **7 day** after installing, 0 otherwise

## Insights
- retention_1 differs by 0.6% between AB groups, with gate_30 higher. But statistically, there is 95.8% chance that the difference between AB groups is above 0%.

- Similarly for retention_7, it differs by 0.8% with gate_30 higher. But statistically, there is 99.8% chance that the difference between AB groups is above 0%.

## Conclusion
Despite popular convention *The later the gate, the higher the retention rate*, data shows the opposite. From my analysis, retention rate is much higher when the gate is at level 30.

One possible explanation is that, being forced to be away from the game earlier at level 30 maybe helpful to prevent an user exhausted from the game to some extent. The surge of wanting to play after some time maybe stronger than keep playing it for a long time. Hence, it is crucial for the company to set an appropriate amount of wait time.

## Limitations and Future steps
One limitation is that, this data doesn't include demographics. Hence, the initial assignment of AB group may not be random enough. In the future, demographic data can be incorporated to run a more thorough AB test. From there, we can quantify the impact of gate for different groups of users.

Moreover, in the future, we can test the appropriate duration for the wait time in order to maximize retention rate.
