# 存储与取出机制

网络在存储或取出物品时，都会遵循以下机制：

## 存储

物品在存储到网络中时，网络会先寻找与[网络监视器](./Network-Monitor)连接的存储。如果存储里是空的，或没有指定类型，那么网络不会向这个存储里面放入物品（不用担心存储单元里出现一把钻石镐）。如果有2个存储单元的物品类型是相同的，那么网络会随机挑选一个放入物品。

如果以上部分不适用，那么网络会开始寻找可用的[网络单元](./Network-Cell)，并优先寻找未满的物品组。如果没有可以补充的物品组，网络会寻找空位来放入物品。

## 取出

网络会优先从[网络单元](./Network-Cell)中取出物品。

如果以上部分不适用，网络会从所有[自动合成机](./Network-Autocrafters)中取出可用的物品。

如果以上部分不适用，网络会从与[网络监视器](./Network-Monitor)连接的存储中取出物品。

如果有必要，网络会从多个地方取出物品来满足需求。