---
description: //wand，这是操作得以成立的前提
---

# 选区和操作

### 在一切之前，先学两个指令

{% hint style="info" %}
//undo可执行撤销操作，用法是//undo \[步数\]，步数不填默认撤销一步。但是：撤销是有次数限制的！尤其是使用笔刷时请务必小心谨慎！

//redo \[步数\] 可重做被撤销的操作
{% endhint %}

## 选区

{% embed url="https://www.bilibili.com/video/av90288829" %}

### 选择模式

| 选择模式 | 指令 |
| :--- | :--- |
| 长方体选择模式 | //sel cuboid |
| 长方体扩大选择模式 | //sel extend |
| 多边形选择模式 | //sel poly |
| 椭球选择模式 | //sel ellipsoid |
| 球体选择模式 | //sel sphere |
| 圆柱体选择模式 | //sel cyl |
| 多面体选择模式 | //sel convex |

### 选择方式

| 选择方式 | 指令 |
| :--- | :--- |
| 木斧选区 | //wand |
| 选择你当前位置（下半身） | //pos1 //pos2 |
| 选择准星所指 | //hpos1 //hpos2 |

### 其他指令

| 操作 | 指令 |
| :--- | :--- |
| 取消选区 | //sel |

## 操作

| 操作 | 指令 |
| :--- | :--- |
| 将选区内全部设置为一种方块 | //set &lt;方块&gt; |
| 替换 | //replace \[原方块（不填为所有非空气方块）\] &lt;新方块&gt; |
| 围墙 | //walls &lt;方块&gt; |
| 火柴盒子 | //outline &lt;方块&gt; |
| 覆盖 | //overlay &lt;方块&gt; |
| 堆叠 | //stack &lt;堆叠次数&gt; \[方向\] |
| 移动 | //move &lt;距离&gt; \[方向\] \[填充方块\] |
| 平滑 | //smooth &lt;迭代次数&gt; |
| 自然化 | //naturalize |
| 使选区内的东西空心 | //hollow |
| 修改生物群系 | //setbiome &lt;生物群系&gt;（//biomelist &lt;页码&gt;可查看所有生物群系） |
| 在pos1和pos2之间连线 | //line &lt;ID&gt; &lt;宽度&gt; |
|  |  |

* 方向的写法：north, south, west, east, up, down，如果不填则默认为你的朝向。（可以简写为n,s,w,e,u,d）
* move的特殊参数：在//move之后，距离之前，写上一个 -s，选区会跟随移动。（十分常用）例如：//move -s 2 up
* 可以用hand表示你手持的方块，试试//set hand
* 虽然有生成花草和树木的指令但是不建议使用，之后会介绍更好的方法。
* stack大法好！

{% hint style="info" %}
重点1：可以填写多个方块，用半角逗号隔开。

重点2：可以设置每种方块出现的概率，只需要在方块前面加上百分比，概率之和不需要恰好为100%，会进行加权平均。

以上两点在绝大部分需要填写方块的场合都能使用
{% endhint %}

{% hint style="info" %}
重点3：生物群系在修改后需要重新进入该地图才会在客户端生效。
{% endhint %}

