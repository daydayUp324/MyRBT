# MyRBT

主要用于自己实现 `Red-Black-Tree`，并测试其对应的性能

## 红黑树

### 概念

「红黑树」是一种特定类型的二叉树，它是在计算机科学中用来组织数据比如数字的块的一种结构。 

「红黑树」是一种平衡二叉查找树的变体，它的左右子树高差有可能大于 1，所以「红黑树」不是严格意义上的「平衡二叉树（AVL）」，但 对之进行平衡的代价较低， 其平均统计性能要强于 AVL 。 

由于每一棵「红黑树」都是一颗「二叉排序树」，因此，在对「红黑树」进行查找时，可以采用运用于普通「二叉排序树」上的查找算法，在查找过程中不需要颜色信息。

### 定义

1. 全部节点只能是红色或者黑色。
2. 根节点是黑色。
3. 所有叶子节点都是黑色，叶子是 NIL 节点。
4. 每一个红色节点的两个叶子节点都是黑色的。（从每一个叶子节点到根的所有路径上不能有两个连续的红色节点）。
5. 从任一节点到其每一个叶子的所有路径都包含相同数目的黑色节点。

### 性质

从根到叶子的最长的可能路径不多于最短的可能路径的两倍长

简单证明：

假设从根节点到某一个叶子节点的最短的路径长度为 $k$，则此时最坏的情况是，这 $k$ 长度的路径和中都是「黑色节点」，那么最长的情况就是，每两个黑色节点中有一个红色节点，那么就会多出 $k - 1$ 个「红色节点」，即最长的路径长度不会超过 $2 * k - 1$。

### 平衡操作

#### 插入操作


#### 删除操作



