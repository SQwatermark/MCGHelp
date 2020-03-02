---
description: 地皮（考核世界）使用PlotSquared插件
---

# 地皮

{% embed url="http://mineplugin.org/PlotSquared" %}

{% embed url="https://github.com/IntellectualSites/PlotSquared/wiki" %}

## 基础使用说明

绝大部分指令需要你站在地皮上使用

不想看下面一大段就只记住三个指令就好了，/plot c领取地皮，/plot home返回地皮，/plot help获取帮助

### 领取和删除地皮

#### /plot claim，/plot auto

claim为领取脚下的地皮，auto是由系统分配一个地皮并将你传送过去。/plot claim可简写为/plot c，妖精可以自主领取地皮但只能领取一块（实际上妖精有整个地皮基础权限包）

#### /plot setowner &lt;玩家&gt;

设置地皮主人

#### /plot delete，/plot clear

delete表示删除地皮，clear表示清空地皮。delete是把地皮还原成无主的空白地皮，所以请不要随意使用此指令。（管理员是可以删除或清空别人的地皮的）

### 移动地皮

#### /plot swap &lt;X,Z&gt;

将当前地皮和指定坐标（地皮的编号）的地皮交换位置（未测试，慎用）

#### /plot move &lt;X,Z&gt;

将当前地皮移动到指定坐标（未测试，慎用）

### 访问地皮

#### /plot visit &lt;玩家名\|地皮名&gt;

访问别人的地皮

#### /plot home \[地皮名\]

如果你有多个地皮的话，仅输入/plot home只能到达指定地皮，这个指令本质上和访问地皮是同一个指令，所以输入/plot visit也可以回到自己的地皮。

#### /plot sethome

设置家

#### /plot middle

传送到地皮中央，强迫症福利（然而mcg的地皮是偶数格）

### 设置地皮属性

/plot alias

/plot setflag

/plot done

/plot continue

### 设置权限

#### /plot add &lt;player\|\*&gt;

允许玩家在地皮主人在线时建造

#### /plot trust &lt;player\|\*&gt;

允许玩家在地皮主人不在线时建造

#### /plot remove

取消该玩家在此地皮的权限

#### /plot deny

禁止玩家进入和移动

/plot merge

/plot unlink

/plot setdescription

/plot toggle



