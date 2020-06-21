第二周学习笔记

一、哈希表、映射、集合

哈希表（Hash table），也叫散列表，是根据关键码值（Keyvalue）而直接进行访问的数据结构。
它通过把关键码值映射到表中一个位置来访问记录，以加快查找的速度。
这个映射函数叫作散列函数（Hash Function），存放记录的数组叫作哈希表（或散列表）。

Java code
•	Map：key-value对，key不重复
-	new HashMap() / new TreeMap()
-	map.set(key, value)
-	map.get(key)
-	map.has(key)
-	map.size()
-	map.clear() 
•	Set：不重复元素的集合
-	new HashSet() / new TreeSet()
-	set.add(value)
-	set.delete(value)
-	set.hash(value)

二、树、二叉树、二叉搜索树

Linked List 是特殊化的 Tree，Tree 是特殊化的 Graph

二叉树遍历 Pre-order/In-order/Post-order
1.	前序（Pre-order）：根-左-右 
2.	中序（In-order）：左-根-右 
3.	后序（Post-order）：左-右-根

二叉搜索树 Binary Search Tree

二叉搜索树，也称二叉搜索树、有序二叉树（Ordered Binary Tree）、排序二叉树（Sorted Binary Tree），是指一棵空树或者具有下列性质的二叉树：
1.	左子树上所有结点的值均小于它的根结点的值；
2.	右子树上所有结点的值均大于它的根结点的值；
3.	以此类推：左、右子树也分别为二叉查找树。 （这就是 重复性！）

二叉搜索树常见操作
1.	查询 
2.	插入新结点（创建） 
3.	删除 

牢记：树的面试题解法一般都是递归！！！

三、堆 Heap 和 二叉堆 Binary Heap

Heap：可以迅速找到一堆数中的最大或者最小值的数据结构，常见的堆有二叉堆、斐波那契堆。
根节点最大的堆叫做大顶堆或者大根堆，根节点最小的堆叫做小顶堆或者小根堆。

二叉堆：通过完全二叉树来实现（注意，不是二叉搜索树）。
二叉大顶堆：1、是一颗完全树；2、树中任意节点的值总是 >= 其子节点的值。

四、图

图的表示与分类：无向无权图、有向无权图、无向有权图

基于图常见的算法：
1、DFS 深度优先搜索算法
2、BFS 广度优先搜索算法

太南了，快肝不动了！怀挺~
