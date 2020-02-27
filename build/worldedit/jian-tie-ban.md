# 剪贴板

## 基本操作

| 操作 | 指令 |
| :--- | :--- |
| 复制 | //copy |
| 剪切 | //cut \[填充方块\] |
| 粘贴 | //paste \[-a\] |
| 旋转 | //rotate &lt;角度&gt; |
| 翻转 | //flip \[-p\] \[方向\] |

{% hint style="info" %}
1. 复制粘贴操作的原点是你的站位
2. 旋转和翻转仅针对剪贴板，你必须先进行//copy或//cut将选区存储进剪贴板，操作完成后//paste放出。
{% endhint %}

### 粘贴

可选参数 -a 表示忽视剪贴板中的空气方块

### 旋转

时代变了，旋转角度不再受到90度的整数倍的限制，而且可以绕三个轴旋转。格式为//rotate X Y Z，建议一次只旋转一个轴。

## 进阶：schematic文件

| 操作 | 指令 |
| :--- | :--- |
| 获取schematic列表 | //schematic list |
| 读取schematic | //schematic load 文件名 |
| 将当前剪贴板保存为schematic | //schematic save 文件名 |

{% hint style="info" %}
schematic保存在服务器文件夹内，且只能从服务器文件夹内读取。所有使用者共享一个schematic库，所以务必科学命名文件。建议文件名以个人ID缩写开头。
{% endhint %}

