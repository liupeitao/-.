# **迪杰斯特拉算法** (Dijkstra algorithm)

### 算法提出者简介

**Edsger Wybe Dijkstra** : 1972年获得图灵奖.

-   提出了目前在[离散数学](https://zh.wikipedia.org/wiki/离散数学)中应用广泛的[最短路径算法](https://zh.wikipedia.org/wiki/Dijkstra算法)（Dijkstra's Shortest Path First Algorithm）
-   为解决[操作系统](https://zh.wikipedia.org/wiki/操作系统)中资源分配问题，提出[银行家算法](https://zh.wikipedia.org/wiki/银行家算法)。

----

### 算法内容

Dijkstra algorithm 是找到*带权图*中给定节点到其他各个节点的的最短路径算法![Dijkstra_Animation](/Users/liupeitao/Desktop/Dijkstra_Animation.gif)

*   !!! **无权图中最短路径,是经过的边的个数, 在带权图中是经过边的权值之和**.

### 一些思考 🤔 最容易想到的解法.

如上图, 如何找出从a到b的最短路径?

假如能找到从点a到点b所有路径, 算出每条路径的总权值, 权值最小的就是 **最短路径**.

*    怎么才能找到两个节点之间的所有通路 ?  时间复杂度怎样? 是不是太慢?
*   节点少很容易看出来, 几十上百个呢?

**最容易想到的方法一般都是: 暴力穷举法 , 利用计算机天赋 *[1)速度快2)不出错]* 找出所有可能再从所有可能中筛选,得出最终结果.**

------

我在a点, 我只能看到和a相连的⑥, ③, ②.所以 (⑥,14), (③, 9 ),(②, 7). 

*   只能看到(只关注)直接相连的节点, 这样有什么好处?  
*   (⑥,14) 表示a到节点⑥的距离是14. 下面👇🏻还会用到***R(③*** )表示a到③, 距离隐式给出.

 

 
