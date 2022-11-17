# 《红色警戒3》三国杀游戏教程

这是一个《红色警戒3》的新游戏模式名为「三国杀」，它允许五位玩家（最好是人类）游玩。在这个模式中，玩家需要扮演不同角色并且完成不同目标来取得胜利。

## 语言

[English](../README.md) | 简体中文 | [繁體中文](./READMES/README.cht.md)

## 怎么玩

### 在游戏前

游戏由五人进行。每位玩家随机地取得以下身份之一：

- 主公 x 1, 
- 忠臣 x 1, 
- 反贼 x 2, 
- 内奸 x 1. 

主公总是在地图最中心。其他玩家的位置是随机分配的。

四种身份被印在雷达的四角。如果你取得了一种身份，在对应的角落附近的地图会被揭示。只有你可以看到你的身份揭示。比如说，在图1，左下角的地图被揭示了，这说明我在游戏中扮演反贼。

![Figure 1](../Figures/Figure-1.1.png)

### 在游戏中

在地图上有几处永久的揭示，它们帮助你搞清楚战场上的局势。

当一名玩家被杀死，广播会通告所有玩家一名对应身份的玩家被击杀，并且与他的身份对应的地图角落会被永久揭示。比如说，在图2，忠臣被杀死了，广播通知了他的死讯，忠臣的地图角落被揭示了。

![Figure 2](../Figures/Figure-1.2.png)

### 游戏结束

对不同身份而言，游戏的目标是不同的：

- 反贼必须杀死主公；
- 主公和忠臣必须杀死反贼和内奸；
- 内奸必须杀死所有角色，主公是最后一个被杀死的。

这里有一个目标更清晰的版本：

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

如果任何一位或一组玩家完成了他，她或他们的目标，他，她或他们将胜利，并且其他玩家将失败。比如说，在图3，反贼杀死了主公，反贼们胜利了。

![Figure 3](../Figures/Figure-1.3.png)

注意：如果内奸杀死了反贼、主公，但是留下了忠臣还活着，内奸没有获胜。
