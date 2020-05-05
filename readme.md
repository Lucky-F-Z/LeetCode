## Leetcode

#### 位运算	

[解法与总结]()

| No.         | Title                                                        | Remark                                                       |
| ----------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 136.        | [只出现一次的数字](https://leetcode-cn.com/problems/single-number/) | 直接异或                                                     |
| 137.        | [只出现一次的数字Ⅱ](https://leetcode-cn.com/problems/single-number-ii/) | 1. 二进制表示中的每一位相加并分析。 2. 直接使用位运算（理解有难度，结合自动机） |
| 260.        | [只出现一次的数字 Ⅲ](https://leetcode-cn.com/problems/single-number-iii/) | 分组异或                                                     |
| 318.        | [最大单词长度乘积](https://leetcode-cn.com/problems/maximum-product-of-word-lengths/) | 把字符串映射成26位二进制位，若两个单词无相同字符，则与操作结果为0 |
| 1318.       | [或运算的最小翻转次数](https://leetcode-cn.com/problems/minimum-flips-to-make-a-or-b-equal-to-c/) | 从二进制每一位来模拟或运算即可                               |
| 389.        | [找不同](https://leetcode-cn.com/problems/find-the-difference/) | 使用异或求出出现奇数次的那个字符/数字                        |
| 面试题05.06 | [整数转换](https://leetcode-cn.com/problems/convert-integer-lcci/) | 直接按位比较                                                 |
| 693         | [交替位二进制数](https://leetcode-cn.com/problems/binary-number-with-alternating-bits/) | 按位比较，但是根据题意不能用for循环32位，而是“有效位数”，因此要不断右移 |

#### 二分查找

[解法与总结]()

| No.   | Title                                                        | Remark                                                     |
| ----- | ------------------------------------------------------------ | ---------------------------------------------------------- |
| 1095  | [山脉数组中查找目标值](https://leetcode-cn.com/problems/find-in-mountain-array/) | 三次二分查找（找山顶，再在前后两个有序数组中二分找target） |
| 33.   | [搜索旋转排序数组](https://leetcode-cn.com/problems/search-in-rotated-sorted-array/) | 整个旋转数组是两段有序数组，因此可以进行二分               |
| 34.   | [在排序数组中查找元素的第一个和最后一个位置](https://leetcode-cn.com/problems/find-first-and-last-position-of-element-in-sorted-array/) | 直接找左边界和有边界                                       |
| 35.   | [搜索插入位置](https://leetcode-cn.com/problems/search-insert-position/) | 直接二分查找即可，若找不到，返回值就是插入位置             |
| 1011. | [在D天内送达包裹的能力](https://leetcode-cn.com/problems/capacity-to-ship-packages-within-d-days/) | 本质上是枚举遍历，只不过使用二分进行了优化                 |
| 875.  | [爱吃香蕉的珂珂](https://leetcode-cn.com/problems/koko-eating-bananas/) | 类似1011，本质上是遍历优化                                 |
|       |                                                              |                                                            |
|       |                                                              |                                                            |
|       |                                                              |                                                            |

#### 链表类型题

[解法与总结]()

| No.  | Title                                                        | Remark                                                       |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 21.  | [合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists/) | 简单的双指针依次比较归并                                     |
| 23.  | [合并k个有序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists/) | 在No.21的基础上加上分治策略                                  |
| 61.  | [旋转链表](https://leetcode-cn.com/problems/rotate-list/)    | 先连成环（这步非必须），再添加断点。本质就是找到旋转后的头节点 |
| 206. | [反转链表](https://leetcode-cn.com/problems/reverse-linked-list/) | 迭代法：三指针逐步分析     递归法：输入一个节点 `head`，将「以 `head` 为起点」的链表反转，并返回反转之后的头结点 |
|      |                                                              |                                                              |
|      |                                                              |                                                              |
|      |                                                              |                                                              |



#### 动态规划

[解法与总结]()

| No.  | Title                                                   | Remark                                                 |
| ---- | ------------------------------------------------------- | ------------------------------------------------------ |
| 55   | [跳跃游戏](https://leetcode-cn.com/problems/jump-game/) | dp[i]表示是否能跳到下标为i的元素，可以使用动态规划解决 |
|      |                                                         |                                                        |
|      |                                                         |                                                        |



#### 贪心算法

[解法与总结]()

| No.  | Title                                                        | Remark                                                       |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 45   | [跳跃游戏Ⅱ](https://leetcode-cn.com/problems/jump-game-ii/submissions/) | 贪心思想：每次选择能到达的最远路径，并且方法数+1，在此基础上再跳下一次 |
| 55   | [跳跃游戏](https://leetcode-cn.com/problems/jump-game/)      | 除了使用dp，也可以使用贪心思想：也是尽可能选择最远的跳，维护一个当前可跳最远距离 |
| 1029 | [两地调度](https://leetcode-cn.com/problems/two-city-scheduling/) | 首先将这 2N2N 个人全都安排飞往 BB 市，再选出 NN 个人改变它们的行程，让他们飞往 AA 市。如果选择改变一个人的行程，那么公司将会额外付出 price_A - price_B 的费用，所以只要这部分最小即可 |
|      |                                                              |                                                              |
|      |                                                              |                                                              |



#### 二叉树及树专题

[解法与总结]()

| No.  | Title                                                        | Remark                                                       |
| ---- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 98   | [验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree/) | 中序遍历满足递增才是二叉搜索树                               |
| 94   | [二叉树中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/) | 在中序遍历中，每个节点也会访问两次，第一次是入栈且不输出，第二次出栈 输出 |
| 144  | [二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal/) | 在先序遍历中，每个节点会被访问两次，第一次是入栈，此时就输出，第二次是出栈 |
| 145  | [二叉树的后序遍历](https://leetcode-cn.com/problems/binary-tree-postorder-traversal/) | 在后序遍历中，每个节点要访问三次<br/>第一次：第一次访问，第一次入栈，不输出<br/>第二次：第二次访问，第一次出栈，此时也不输出，而是进行第二次入栈，然后访问该节点的右节点<br/>第三次：第三次访问，是当访问完了某个节点的右子树，再次回到该节点时，即第二次出栈，此时输出 |
| 501  | [二叉搜索树中的众数](https://leetcode-cn.com/problems/find-mode-in-binary-search-tree/) | 先中序遍历，再对数组求众数                                   |
|      |                                                              |                                                              |
|      |                                                              |                                                              |
