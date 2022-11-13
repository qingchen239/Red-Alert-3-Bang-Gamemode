# Red Alert 3 Bang Game Tutorial

This is a new game method named "Bang Game" for Red Alert 3, which is allowed five players(better be human) to play. In this game method, gamers should play different roles, and accomplish different goals to achieve victory. 

## Languages

English | [简体中文](./READMES/README.chs.md) | [繁體中文](./READMES/README.cht.md)

## How to play

### Before the game

The game is played by five players. Each player takes one of the following roles randomly: 

- Sheriff x 1, 
- Deputy Sheriff x 1, 
- Outlaws x 2, 
- Renegade x 1. 

The Sheriff is always in the middle of the map. Positions for other players are randomly assigned. 

These four roles are printed on each corner of your radar. If you have taken one role, the map near its corresponding corner is revealed. For example, in figure 1, the bottom-left corner of this map is revealed, which means that I play as one of the Outlaws in this game. 

![Figure 1](./Figures/Figure-1.png)

### During the game

There are a few permanent reveals on the map that helps you to figure out the situation on the battlefield. 

When one player is killed, the broadcast will announce to everyone that a player of a corresponding role has been killed, and the map corner corresponding to his role will be revealed permanently. Only you can see your role revealiation. For example, in figure 2, the deputy has been killed, the broadcast announces his death, and the map corner corresponds to the Deputy has been revealed. 

![Figure 2](./Figures/Figure-2.png)

### End of the game

The objective of the game is different for every role randomly: 

- The Outlaws must kill the Sheriff; 
- The Sheriff and his Deputy must kill the Outlaws and the Renegade. 
- The Renegade must kill all the characters with the Sheriff being the last one dead. 

Here is a much clarity version of the objective. 

```
if Sheriff is dead and more than 1 Outlaws is alive:
	Outlaws win
else if Outlaws are dead and Renegate is dead:
	Sheriff and Deputy win
else if Outlaws are dead and Renegate is dead and Sheriff is dead:
	Renegade wins
else if Sheriff is dead and more than 1 Deputy is alive:
	nobody wins
```

If any one player or group of players has completed his, her, or their objective, he, she, or they will win, and other player players will lose. For example, in figure 3, the Outlaw has killed the Sheriff, and the Outlaws win. 

![Figure 3](./Figures/Figure-3.png)

Caution: If the Renegade kills the Outlaws, and the Sheriff, but leaves the Deputy alive, the Renegade does not win the game. 

