---
description: 推荐的指令会给出用法
---

# 推荐掌握

## powertool

作用：将指令绑定到手持的物品上，手持物品左键一次就相当于输入一遍指令，十分方便。

简写为pt

基础格式：/powertool 指令

示例：手持一个物品输入/powertool bigtree tree，手持此物品左键时，就会由你执行一遍/bigtree tree指令，在准星位置种上一棵树。

特殊格式

* /powertool c:&lt;消息&gt; （说出消息，c表示chat）
* /powertool a:&lt;指令&gt;  （附加一条指令，a表示append） 
* /powertool r:&lt;指令&gt; （移除一条指令，r表示remove）
* /powertool l: （列出所有指令，l表示list）
* /powertool d:（移除所有指令，d表示delete）

## ptime和pweather

作用：p表示player，可以设置玩家所看到的时间和天气而不会改变服务器的时间和天气。这样施工或者拍风景时就不需要改世界时间或者嗑药了，十分方便。

格式：

* /ptime \[list\|reset\|day\|night\|dawn\|17:30\|4pm\|4000ticks\] \[player\|\*\]
* /pweather \[list\|reset\|storm\|sun\|clear\] \[player\|\*\]

示例：

* /ptime day，将自己的时间设置为6点（0tick）
* /ptime night SQwatermark，将SQwatermark的时间设置成晚上

## remove

移除实体

