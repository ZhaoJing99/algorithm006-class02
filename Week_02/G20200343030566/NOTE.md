学习笔记
recursive 递归四步骤
    1.terminator 终止条件
    2.Process Logic 程序逻辑
    3.Drill Down 下沉
    4.reverse status 返回
散列表：
    HashTable又名哈希表，以键值对的形式进行存储的数据结果，通过将Key经过hash算法后映射到表中的一个位置来进行访问记录，其底层数据结构是数组，散列表借用了数组支持按照下标随机访问的特性，时间复杂度是O(1),
业界代表性哈希算法：
    MD5,SHA,CRC,
哈希冲突：
    哈希算法产生的哈希值的长度是固定且有限的，因此要找到一个不同的key对应的散列值不一样的哈希函数，几乎不可能，且因为底层数组的存储空间有限，也会加大散列冲突的概率
哈希冲突解决方案：
    1.开放寻址法：出现哈希冲突，重新寻找数组空闲位置
    2.链表法：散列值相同的元素放入相同槽位的链表中，插入时间复杂度O(1),删除或查找O(k),k为链表的长度
    3.双重散列法：当第一次产生冲突时，再次调用哈希函数进行计算hash值

Hash的应用：
    1.文件校验
    2.数字签名
    3.鉴权协议
    4.负载均衡
    5.数据分片
    6.分布式存储
    
二叉树：
    非线性表结构，每个结点最多有两个子树的树结构。通常子树被称作“左子树”（left subtree）和“右子树”（right subtree）
满二叉树：
    叶子节点全部都在最底层，除了叶子节点之外，每个节点都有左右两个子节点，这种二叉树叫满二叉树
完全二叉树：
    叶子节点全部都在最底层，最后一层的叶子节点都靠左排列，并且除了最后一层，其它层的节点个数全部都要达到最大
    
存储二叉树的方式：
    1.基于指针或者引用的二叉链式存储法，
    2.基于数组的顺序存储法 父节点的下标位置是i,则左子树的位置存储是：2*i,右子树的位置存储是：2*1+1;
    
二叉树的遍历：
    1.前序遍历:根-->左-->右
    2.中序遍历:左-->根-->右
    3.后序遍历:左-->右-->根

二叉查找树（Binary Search Tree）:
    在树中的任意一个节点，其左子树中的每个节点的值，都要小于根节点的值，其右子树中的每个节点的值，都要大于根节点的值
    
    
Code Review：
    364:少一些辅助性注释
    380:逻辑清晰，总结优秀
    516:思路及分析很不错，整理多语言这一点很不错
    428:注释清晰，工整
    

