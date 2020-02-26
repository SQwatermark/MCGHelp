---
description: 依赖LuckPerms插件
---

# 权限管理

{% embed url="https://pluginscdtribe.github.io/wiki/luckperms/" caption="LuckPerms中文wiki（这里啥都有）" %}

### 常用指令

| 操作 | 指令 |
| :--- | :--- |
| 创建权限组 | /lp creategroup 组名 |
| 删除权限组 | /lp deletegroup 组名 |
| 列出权限组 | /lp listgroups |
| 设置/添加/移除父组 | /lp group/user 组名/玩家名 parent set/add/remove 父组名 |
| 添加/禁用权限 | /lp group/user 组名/玩家名 permission set 权限节点 true/false |
| 取消定义权限 | /lp group/user 组名/玩家名 permission unset 权限节点 |

### 分世界权限

只需要在指令最后加上 world=世界名 即可

例如：/lp user SQwatermark parent set 毛玉 world=plots

SQwatermark在地皮世界的权限就是毛玉了

又例如：/lp group 妖精 permission set gamemode.creative true world=plots

妖精就获得了在地皮世界自由开启创造模式的权限

{% hint style="info" %}
世界名要填写完整，主世界是mcg\_gensokyo而不是gensokyo，一个简单的查看世界原名的方式是看网页地图里的世界名
{% endhint %}

### 网页编辑器

输入/lp editor，将返回的链接复制到剪贴板

![](../../.gitbook/assets/image%20%282%29.png)

![](../../.gitbook/assets/image%20%283%29.png)

用一个靠谱的浏览器打开链接，你就会看到如图所示的编辑器，你可以通过网页编辑所有权限组和所有在线玩家的权限

![](../../.gitbook/assets/image%20%284%29.png)

编辑完之后，点击右上方的保存，在服务器里执行网页返回的指令

![](../../.gitbook/assets/image%20%285%29.png)

显示类似于下方的信息，表示编辑成功，通常会返回有哪些内容出现了变动，但是我并没有改动任何权限，所以返回的是这样的一段话

![](../../.gitbook/assets/image%20%286%29.png)

有时你只想编辑某个权限组或者某个玩家的权限，可以执行这样的指令：

/lp group\|player 权限组\|玩家名 editor

这样网页编辑器里就只有指定的组/玩家了

### 权限优先级的计算

* 世界特定的权限是会覆盖通用/全局权限设置的
* 临时权限将会覆盖非临时权限（本服没有临时权限）
* 如果同时有两个节点相同、但时长不同的临时权限，时间较长的会覆盖时间较短的
* 更加具体的通配符权限将覆盖不具体的通配符权限

例如：一个用户拥有权限“luckperms.”并且设置为true，但是“luckperms.user.”权限却设置为false， 那么所有玩家的权限都将被设置为false！ 因为尽管“luckperm.”有更加通用的通配符，但是他没有“luckperms.user.”具体。

* 玩家的权限优先于玩家所属权限组的权限，权限组的权限优先于其父组的权限



