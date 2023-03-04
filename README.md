# Red Alert 3 "Bang!" Gamemode Tutorial

This is a new gamemode named "Bang!" for Red Alert 3, which is allowed five players(better be human) to play. In this game method, gamers should play different roles, and accomplish different goals to achieve victory. 

## Languages

English | [简体中文](./READMES/README.chs.md) | [繁體中文](./READMES/README.cht.md)

## How to play

### Before the game

The game is played by five players. Each player takes one of the following roles: 

- Sheriff x 1, 
- Deputy Sheriff x 1, 
- Outlaws x 2, 
- Renegade x 1. 

The Sheriff is always in the middle of the map. Positions for other players are randomly assigned. 

These four roles are printed on each corner of your radar. If you have taken one role, the map near its corresponding corner is revealed. Only you can see your role revealation. For example, in figure 1, the bottom-left corner of this map is revealed, which means that I play as one of the Outlaws in this game. 

![Figure 1](./Figures/Figure-1.1.png)

### During the game

There are a few permanent reveals on the map that helps you to figure out the situation on the battlefield. 

When one player is killed, the broadcast will announce to everyone that a player of a corresponding role has been killed, and the map corner corresponding to his role will be revealed permanently. Everyone can see his role revealiation. For example, in figure 2, the deputy has been killed, the broadcast announces his death, and the map corner corresponds to the Deputy has been revealed. 

![Figure 2](./Figures/Figure-1.2.png)

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

__Caution: If someone quits the game, he will be considered killed. For example, if the Deputy and the Renegade are alive and the Sheriff quits, Outlaws will win the game. Quitting the game before really being killed is bad behavior.__

__Caution: If the Renegade kills the Outlaws, and the Sheriff, but leaves the Deputy alive, the Renegade does not win the game.__

If any one player or group of players has completed his, her, or their objective, he, she, or they will win, and other player players will lose. For example, in figure 3, the Outlaw has killed the Sheriff, and the Outlaws win. 

![Figure 3](./Figures/Figure-1.3.png)

## Derivatives rules

Everyone is free to modify the maps in this repository and to distribute modified and therefore derivative works, __when following these rules__:

- To note to other people that that map is not the original version. 

- Let other people know who modified this map and how to connect to you. 

- Do not use the same name with other derivatives. (You may add your own name on the map name. )

## Connect with me

Discord: Qing Chen#1901
