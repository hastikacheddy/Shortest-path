# Shortest-path · 最短路径可视化

[English](README.md) | 简体中文

一个带图形界面（GUI）的 Java 程序：用户输入节点数量后，程序会生成对应的图，求出遍历所有节点的最短路径，并显示路径和总距离。

## 工作原理

1. 程序提示用户输入节点数量。
2. 为每个节点随机生成 x、y 坐标。
3. 用这些节点构建一个**完全图**，并以**邻接矩阵**的形式存储。
4. 使用 **Floyd–Warshall 算法**计算任意两个节点之间的最短路径。
5. 生成所有节点的**全排列**，每种排列代表一种访问节点的顺序。
6. 一条路径的代价等于相邻两个节点之间最短路径长度之和。
7. 逐一比较各排列的代价，代价最小的排列即为最短路径。
8. GUI 绘制并显示该路径，同时输出路径顺序和总长度。

> 注：由于需要枚举全排列，时间复杂度为 O(n!)，适合节点数量较少的演示场景。

## 运行截图

1. 输入 4 个节点时的输出：

   ![image](https://github.com/hastikacheddy/Shortest-path/assets/59787014/39d1293f-3e36-465f-af9d-beb4e8028670)

2. 输入 9 个节点时的输出：

   ![image](https://github.com/hastikacheddy/Shortest-path/assets/59787014/584b23f2-36fd-45e8-9f86-778d252fb8bc)

## 项目结构

| 文件 | 说明 |
| --- | --- |
| `shortest-path/GraphDraw.java`、`GraphDraw2.java` | 图形界面与路径绘制 |
| `shortest-path/GFG.java` | 最短路径算法实现 |

## 运行方法

```bash
cd shortest-path
javac *.java
java GraphDraw
```
