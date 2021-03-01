## 相关介绍
这是一个简易的LeetCode自动统计程序, 可自动统计最近提交通过的题目, 并以Markdown的形式展示相关的数据。
根据个人需求, 我只重点获取**提交次数**和**重刷次数**这两个指标, 目的是为了更好地辅助做题。
## 使用教程
1. Fork本仓库
2. 配置GitHub Actions所需的参数
    - 点击仓库下的Settings->Secrets->New repository secret, 分别添加以下secret
        - Name:LEETCODE_EMAIL  Value:你的LeetCode账号
        - Name:LEETCODE_PASSWORD  Value:你的LeetCode密码
    - 点击[tokens](https://github.com/settings/tokens)->Generate new token
        - Note:GITHUB_TOKEN
        - Select scopes:建议全部勾选
    - 修改[action.yml](.github/workflows/action.yml)文件的第`42行`, 将`email`更改为你的GitHub邮箱地址
    - 修改[action.yml](.github/workflows/action.yml)文件的第`43行`, 将`name`更改为你的GitHub用户名
3. 默认配置为12小时更新一次，可根据需求修改[action.yml](.github/workflows/action.yml)文件的第`6行`
## 补充说明
如有其他需求, 欢迎提交PR。


> 重刷次数的计算规则为: 累计所有提交通过且互为不同一天的记录次数

| 最近提交时间 | 题目 | 题目难度 | 提交次数| 重刷次数 |
| ---- | ---- | ---- | ---- | ---- |
| 2021-02-28 13:54 | [#896 单调数列](https://leetcode-cn.com/problems/monotonic-array) | EASY | 4 | 1 |
| 2021-02-27 10:23 | [#415 字符串相加](https://leetcode-cn.com/problems/add-strings) | EASY | 3 | 1 |
| 2021-02-27 09:04 | [#160 相交链表](https://leetcode-cn.com/problems/intersection-of-two-linked-lists) | EASY | 1 | 1 |
| 2021-02-26 16:01 | [#142 环形链表 II](https://leetcode-cn.com/problems/linked-list-cycle-ii) | MEDIUM | 4 | **2** |
| 2021-02-26 15:27 | [#96 不同的二叉搜索树](https://leetcode-cn.com/problems/unique-binary-search-trees) | MEDIUM | 5 | **2** |
| 2021-02-26 15:10 | [#241 为运算表达式设计优先级](https://leetcode-cn.com/problems/different-ways-to-add-parentheses) | MEDIUM | 6 | **2** |
| 2021-02-25 03:56 | [#931 下降路径最小和](https://leetcode-cn.com/problems/minimum-falling-path-sum) | MEDIUM | 2 | 1 |
| 2021-02-24 13:18 | [#832 翻转图像](https://leetcode-cn.com/problems/flipping-an-image) | EASY | 1 | 1 |
| 2021-02-24 12:48 | [#24 两两交换链表中的节点](https://leetcode-cn.com/problems/swap-nodes-in-pairs) | MEDIUM | 1 | 1 |
| 2021-02-23 10:24 | [#1052 爱生气的书店老板](https://leetcode-cn.com/problems/grumpy-bookstore-owner) | MEDIUM | 1 | 1 |
| 2021-02-23 09:31 | [#460 LFU 缓存](https://leetcode-cn.com/problems/lfu-cache) | HARD | 3 | 1 |
| 2021-02-23 03:50 | [#23 合并K个升序链表](https://leetcode-cn.com/problems/merge-k-sorted-lists) | HARD | 3 | **2** |
| 2021-02-22 15:16 | [#25 K 个一组翻转链表](https://leetcode-cn.com/problems/reverse-nodes-in-k-group) | HARD | 6 | **2** |
| 2021-02-22 07:44 | [#剑指 Offer 22 链表中倒数第k个节点](https://leetcode-cn.com/problems/lian-biao-zhong-dao-shu-di-kge-jie-dian-lcof) | EASY | 1 | 1 |
| 2021-02-22 01:44 | [#1541 平衡括号字符串的最少插入次数](https://leetcode-cn.com/problems/minimum-insertions-to-balance-a-parentheses-string) | MEDIUM | 5 | 1 |
| 2021-02-22 01:05 | [#921 使括号有效的最少添加](https://leetcode-cn.com/problems/minimum-add-to-make-parentheses-valid) | MEDIUM | 2 | 1 |
| 2021-02-22 00:58 | [#20 有效的括号](https://leetcode-cn.com/problems/valid-parentheses) | EASY | 6 | **2** |
| 2021-02-21 12:43 | [#剑指 Offer 68 - I 二叉搜索树的最近公共祖先](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-de-zui-jin-gong-gong-zu-xian-lcof) | EASY | 1 | 1 |
| 2021-02-21 12:37 | [#剑指 Offer 68 - II 二叉树的最近公共祖先](https://leetcode-cn.com/problems/er-cha-shu-de-zui-jin-gong-gong-zu-xian-lcof) | EASY | 1 | 1 |
| 2021-02-21 11:07 | [#剑指 Offer 32 - I 从上到下打印二叉树](https://leetcode-cn.com/problems/cong-shang-dao-xia-da-yin-er-cha-shu-lcof) | MEDIUM | 2 | 1 |
| 2021-02-21 10:03 | [#958 二叉树的完全性检验](https://leetcode-cn.com/problems/check-completeness-of-a-binary-tree) | MEDIUM | 1 | 1 |
| 2021-02-21 06:19 | [#1438 绝对差不超过限制的最长连续子数组](https://leetcode-cn.com/problems/longest-continuous-subarray-with-absolute-diff-less-than-or-equal-to-limit) | MEDIUM | 4 | 1 |
| 2021-02-20 08:08 | [#300 最长递增子序列](https://leetcode-cn.com/problems/longest-increasing-subsequence) | MEDIUM | 8 | **2** |
| 2021-02-20 03:47 | [#151 翻转字符串里的单词](https://leetcode-cn.com/problems/reverse-words-in-a-string) | MEDIUM | 2 | 1 |
| 2021-02-20 03:16 | [#LCP 24 数字游戏](https://leetcode-cn.com/problems/5TxKeK) | HARD | 4 | 1 |
| 2021-02-19 14:12 | [#33 搜索旋转排序数组](https://leetcode-cn.com/problems/search-in-rotated-sorted-array) | MEDIUM | 1 | 1 |
| 2021-02-19 11:08 | [#92 反转链表 II](https://leetcode-cn.com/problems/reverse-linked-list-ii) | MEDIUM | 2 | 1 |
| 2021-02-19 09:52 | [#剑指 Offer 24 反转链表](https://leetcode-cn.com/problems/fan-zhuan-lian-biao-lcof) | EASY | 3 | **2** |
| 2021-02-19 02:19 | [#面试题 02.06 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list-lcci) | EASY | 3 | 1 |
| 2021-02-17 05:55 | [#21 合并两个有序链表](https://leetcode-cn.com/problems/merge-two-sorted-lists) | EASY | 1 | 1 |
| 2021-02-17 05:27 | [#566 重塑矩阵](https://leetcode-cn.com/problems/reshape-the-matrix) | EASY | 1 | 1 |
| 2021-02-16 09:20 | [#54 螺旋矩阵](https://leetcode-cn.com/problems/spiral-matrix) | MEDIUM | 5 | 1 |
| 2021-02-15 14:20 | [#53 最大子序和](https://leetcode-cn.com/problems/maximum-subarray) | EASY | 5 | **3** |
| 2021-02-15 14:16 | [#200 岛屿数量](https://leetcode-cn.com/problems/number-of-islands) | MEDIUM | 5 | **2** |
| 2021-02-14 16:26 | [#485 最大连续 1 的个数](https://leetcode-cn.com/problems/max-consecutive-ones) | EASY | 3 | 1 |
| 2021-02-14 13:03 | [#95 不同的二叉搜索树 II](https://leetcode-cn.com/problems/unique-binary-search-trees-ii) | MEDIUM | 3 | 1 |
| 2021-02-13 16:58 | [#623 在二叉树中增加一行](https://leetcode-cn.com/problems/add-one-row-to-tree) | MEDIUM | 2 | 1 |
| 2021-02-13 16:10 | [#448 找到所有数组中消失的数字](https://leetcode-cn.com/problems/find-all-numbers-disappeared-in-an-array) | EASY | 2 | 1 |
| 2021-02-13 15:07 | [#337 打家劫舍 III](https://leetcode-cn.com/problems/house-robber-iii) | MEDIUM | 6 | **2** |
| 2021-02-12 03:30 | [#863 二叉树中所有距离为 K 的结点](https://leetcode-cn.com/problems/all-nodes-distance-k-in-binary-tree) | MEDIUM | 1 | 1 |
| 2021-02-11 09:06 | [#1145 二叉树着色游戏](https://leetcode-cn.com/problems/binary-tree-coloring-game) | MEDIUM | 1 | 1 |
| 2021-02-11 07:05 | [#979 在二叉树中分配硬币](https://leetcode-cn.com/problems/distribute-coins-in-binary-tree) | MEDIUM | 1 | 1 |
| 2021-02-10 03:36 | [#987 二叉树的垂序遍历](https://leetcode-cn.com/problems/vertical-order-traversal-of-a-binary-tree) | HARD | 3 | 1 |
| 2021-02-10 01:52 | [#655 输出二叉树](https://leetcode-cn.com/problems/print-binary-tree) | MEDIUM | 7 | **2** |
| 2021-02-10 00:31 | [#98 验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree) | MEDIUM | 9 | **2** |
| 2021-02-09 03:11 | [#124 二叉树中的最大路径和](https://leetcode-cn.com/problems/binary-tree-maximum-path-sum) | HARD | 7 | **2** |
| 2021-02-08 13:46 | [#753 破解保险箱](https://leetcode-cn.com/problems/cracking-the-safe) | HARD | 5 | 1 |
| 2021-02-08 03:56 | [#468 验证IP地址](https://leetcode-cn.com/problems/validate-ip-address) | MEDIUM | 3 | **2** |
| 2021-02-07 13:48 | [#5 最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring) | MEDIUM | 10 | **2** |
| 2021-02-07 13:32 | [#121 买卖股票的最佳时机](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock) | EASY | 4 | **2** |
| 2021-02-07 13:31 | [#100 相同的树](https://leetcode-cn.com/problems/same-tree) | EASY | 4 | **3** |
| 2021-02-06 14:49 | [#638 大礼包](https://leetcode-cn.com/problems/shopping-offers) | MEDIUM | 5 | 1 |
| 2021-02-05 06:51 | [#971 翻转二叉树以匹配先序遍历](https://leetcode-cn.com/problems/flip-binary-tree-to-match-preorder-traversal) | MEDIUM | 9 | **2** |
| 2021-02-05 02:31 | [#72 编辑距离](https://leetcode-cn.com/problems/edit-distance) | HARD | 2 | **2** |
| 2021-02-05 02:23 | [#60 排列序列](https://leetcode-cn.com/problems/permutation-sequence) | HARD | 1 | 1 |
| 2021-02-03 16:42 | [#907 子数组的最小值之和](https://leetcode-cn.com/problems/sum-of-subarray-minimums) | MEDIUM | 5 | 1 |
| 2021-02-03 10:59 | [#146 LRU 缓存机制](https://leetcode-cn.com/problems/lru-cache) | MEDIUM | 3 | **2** |
| 2021-02-03 10:18 | [#215 数组中的第K个最大元素](https://leetcode-cn.com/problems/kth-largest-element-in-an-array) | MEDIUM | 1 | 1 |
| 2021-02-03 10:10 | [#1739 放置盒子](https://leetcode-cn.com/problems/building-boxes) | HARD | 4 | 1 |
| 2021-02-03 10:07 | [#22 括号生成](https://leetcode-cn.com/problems/generate-parentheses) | MEDIUM | 2 | **2** |
| 2021-02-02 02:43 | [#85 最大矩形](https://leetcode-cn.com/problems/maximal-rectangle) | HARD | 10 | **4** |
| 2021-02-01 06:59 | [#172 阶乘后的零](https://leetcode-cn.com/problems/factorial-trailing-zeroes) | EASY | 1 | 1 |
| 2021-02-01 05:44 | [#105 从前序与中序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal) | MEDIUM | 2 | **2** |
| 2021-01-31 14:45 | [#剑指 Offer 26 树的子结构](https://leetcode-cn.com/problems/shu-de-zi-jie-gou-lcof) | MEDIUM | 3 | **2** |
| 2021-01-29 10:56 | [#42 接雨水](https://leetcode-cn.com/problems/trapping-rain-water) | HARD | 3 | 1 |
| 2021-01-29 00:17 | [#11 盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water) | MEDIUM | 2 | **2** |
| 2021-01-27 02:36 | [#514 自由之路](https://leetcode-cn.com/problems/freedom-trail) | HARD | 4 | **2** |
| 2021-01-25 14:32 | [#1373 二叉搜索子树的最大键值和](https://leetcode-cn.com/problems/maximum-sum-bst-in-binary-tree) | HARD | 1 | 1 |
| 2021-01-24 13:31 | [#31 下一个排列](https://leetcode-cn.com/problems/next-permutation) | MEDIUM | 8 | **2** |
| 2021-01-21 04:01 | [#714 买卖股票的最佳时机含手续费](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee) | MEDIUM | 6 | **3** |
| 2021-01-15 04:07 | [#895 最大频率栈](https://leetcode-cn.com/problems/maximum-frequency-stack) | HARD | 2 | 1 |
| 2021-01-14 16:53 | [#剑指 Offer 48 最长不含重复字符的子字符串](https://leetcode-cn.com/problems/zui-chang-bu-han-zhong-fu-zi-fu-de-zi-zi-fu-chuan-lcof) | MEDIUM | 2 | **2** |
| 2021-01-13 09:51 | [#684 冗余连接](https://leetcode-cn.com/problems/redundant-connection) | MEDIUM | 2 | 1 |
| 2021-01-13 02:24 | [#剑指 Offer 62 圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof) | EASY | 4 | 1 |
| 2021-01-11 16:44 | [#剑指 Offer 19 正则表达式匹配](https://leetcode-cn.com/problems/zheng-ze-biao-da-shi-pi-pei-lcof) | HARD | 2 | 1 |
| 2021-01-10 14:56 | [#10 正则表达式匹配](https://leetcode-cn.com/problems/regular-expression-matching) | HARD | 5 | 1 |
| 2021-01-09 04:01 | [#7 整数反转](https://leetcode-cn.com/problems/reverse-integer) | EASY | 1 | 1 |
| 2021-01-08 13:05 | [#189 旋转数组](https://leetcode-cn.com/problems/rotate-array) | MEDIUM | 1 | 1 |
| 2021-01-07 15:28 | [#174 地下城游戏](https://leetcode-cn.com/problems/dungeon-game) | HARD | 1 | 1 |
| 2021-01-04 08:44 | [#509 斐波那契数](https://leetcode-cn.com/problems/fibonacci-number) | EASY | 2 | 1 |
| 2021-01-02 11:51 | [#16 最接近的三数之和](https://leetcode-cn.com/problems/3sum-closest) | MEDIUM | 1 | 1 |
| 2021-01-01 11:57 | [#605 种花问题](https://leetcode-cn.com/problems/can-place-flowers) | EASY | 9 | 1 |
| 2021-01-01 05:42 | [#435 无重叠区间](https://leetcode-cn.com/problems/non-overlapping-intervals) | MEDIUM | 3 | 1 |
| 2020-12-30 14:05 | [#1046 最后一块石头的重量](https://leetcode-cn.com/problems/last-stone-weight) | EASY | 1 | 1 |
| 2020-12-30 11:43 | [#1406 石子游戏 III](https://leetcode-cn.com/problems/stone-game-iii) | HARD | 1 | 1 |
| 2020-12-30 06:30 | [#1140 石子游戏 II](https://leetcode-cn.com/problems/stone-game-ii) | MEDIUM | 4 | **2** |
| 2020-12-27 12:46 | [#213 打家劫舍 II](https://leetcode-cn.com/problems/house-robber-ii) | MEDIUM | 3 | 1 |
| 2020-12-27 09:52 | [#205 同构字符串](https://leetcode-cn.com/problems/isomorphic-strings) | EASY | 6 | 1 |
| 2020-12-26 12:52 | [#198 打家劫舍](https://leetcode-cn.com/problems/house-robber) | MEDIUM | 2 | 1 |
| 2020-12-26 08:33 | [#1028 从先序遍历还原二叉树](https://leetcode-cn.com/problems/recover-a-tree-from-preorder-traversal) | HARD | 2 | 1 |
| 2020-12-25 01:55 | [#998 最大二叉树 II](https://leetcode-cn.com/problems/maximum-binary-tree-ii) | MEDIUM | 1 | 1 |
| 2020-12-24 17:33 | [#662 二叉树最大宽度](https://leetcode-cn.com/problems/maximum-width-of-binary-tree) | MEDIUM | 3 | 1 |
| 2020-12-24 16:23 | [#236 二叉树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree) | MEDIUM | 1 | 1 |
| 2020-12-23 15:19 | [#752 打开转盘锁](https://leetcode-cn.com/problems/open-the-lock) | MEDIUM | 1 | 1 |
| 2020-12-23 07:57 | [#64 最小路径和](https://leetcode-cn.com/problems/minimum-path-sum) | MEDIUM | 2 | 1 |
| 2020-12-23 03:54 | [#8 字符串转换整数 (atoi)](https://leetcode-cn.com/problems/string-to-integer-atoi) | MEDIUM | 1 | 1 |
| 2020-12-22 16:15 | [#387 字符串中的第一个唯一字符](https://leetcode-cn.com/problems/first-unique-character-in-a-string) | EASY | 1 | 1 |
| 2020-12-22 16:08 | [#104 二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree) | EASY | 2 | 1 |
| 2020-12-22 12:10 | [#48 旋转图像](https://leetcode-cn.com/problems/rotate-image) | MEDIUM | 1 | 1 |
| 2020-12-18 16:03 | [#389 找不同](https://leetcode-cn.com/problems/find-the-difference) | EASY | 2 | 1 |
| 2020-12-18 15:34 | [#6 Z 字形变换](https://leetcode-cn.com/problems/zigzag-conversion) | MEDIUM | 4 | 1 |
| 2020-12-17 06:51 | [#199 二叉树的右视图](https://leetcode-cn.com/problems/binary-tree-right-side-view) | MEDIUM | 1 | 1 |
| 2020-12-15 16:46 | [#738 单调递增的数字](https://leetcode-cn.com/problems/monotone-increasing-digits) | MEDIUM | 3 | 1 |
| 2020-12-15 14:54 | [#334 递增的三元子序列](https://leetcode-cn.com/problems/increasing-triplet-subsequence) | MEDIUM | 7 | **2** |
| 2020-12-13 14:45 | [#669 修剪二叉搜索树](https://leetcode-cn.com/problems/trim-a-binary-search-tree) | MEDIUM | 2 | 1 |
| 2020-12-13 14:22 | [#814 二叉树剪枝](https://leetcode-cn.com/problems/binary-tree-pruning) | MEDIUM | 2 | 1 |
| 2020-12-11 13:27 | [#877 石子游戏](https://leetcode-cn.com/problems/stone-game) | MEDIUM | 3 | 1 |
| 2020-12-11 12:25 | [#319 灯泡开关](https://leetcode-cn.com/problems/bulb-switcher) | MEDIUM | 1 | 1 |
| 2020-12-11 02:23 | [#36 有效的数独](https://leetcode-cn.com/problems/valid-sudoku) | MEDIUM | 4 | 1 |
| 2020-12-10 17:14 | [#14 最长公共前缀](https://leetcode-cn.com/problems/longest-common-prefix) | EASY | 4 | 1 |
| 2020-12-10 16:58 | [#395 至少有 K 个重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-with-at-least-k-repeating-characters) | MEDIUM | 11 | 1 |
| 2020-12-09 13:22 | [#152 乘积最大子数组](https://leetcode-cn.com/problems/maximum-product-subarray) | MEDIUM | 6 | 1 |
| 2020-12-08 17:12 | [#62 不同路径](https://leetcode-cn.com/problems/unique-paths) | MEDIUM | 2 | **2** |
| 2020-12-08 16:59 | [#378 有序矩阵中第 K 小的元素](https://leetcode-cn.com/problems/kth-smallest-element-in-a-sorted-matrix) | MEDIUM | 9 | **2** |
| 2020-12-06 15:24 | [#118 杨辉三角](https://leetcode-cn.com/problems/pascals-triangle) | EASY | 1 | 1 |
| 2020-12-06 13:03 | [#111 二叉树的最小深度](https://leetcode-cn.com/problems/minimum-depth-of-binary-tree) | EASY | 6 | **2** |
| 2020-12-06 12:53 | [#1306 跳跃游戏 III](https://leetcode-cn.com/problems/jump-game-iii) | MEDIUM | 3 | 1 |
| 2020-12-06 09:30 | [#剑指 Offer 10- II 青蛙跳台阶问题](https://leetcode-cn.com/problems/qing-wa-tiao-tai-jie-wen-ti-lcof) | EASY | 3 | 1 |
| 2020-12-05 14:39 | [#103 二叉树的锯齿形层序遍历](https://leetcode-cn.com/problems/binary-tree-zigzag-level-order-traversal) | MEDIUM | 4 | 1 |
| 2020-12-04 17:28 | [#569 员工薪水中位数](https://leetcode-cn.com/problems/median-employee-salary) | HARD | 2 | 1 |
| 2020-12-04 13:35 | [#1045 买下所有产品的客户](https://leetcode-cn.com/problems/customers-who-bought-all-products) | MEDIUM | 2 | 1 |
| 2020-12-04 11:12 | [#1049 最后一块石头的重量 II](https://leetcode-cn.com/problems/last-stone-weight-ii) | MEDIUM | 1 | 1 |
| 2020-12-04 03:08 | [#474 一和零](https://leetcode-cn.com/problems/ones-and-zeroes) | MEDIUM | 2 | 1 |
| 2020-12-03 17:19 | [#1081 不同字符的最小子序列](https://leetcode-cn.com/problems/smallest-subsequence-of-distinct-characters) | MEDIUM | 1 | 1 |
| 2020-12-03 16:51 | [#321 拼接最大数](https://leetcode-cn.com/problems/create-maximum-number) | HARD | 5 | 1 |
| 2020-12-03 12:42 | [#204 计数质数](https://leetcode-cn.com/problems/count-primes) | EASY | 2 | 1 |
| 2020-12-03 06:02 | [#316 去除重复字母](https://leetcode-cn.com/problems/remove-duplicate-letters) | MEDIUM | 4 | 1 |
| 2020-12-03 02:25 | [#LCP 09 最小跳跃次数](https://leetcode-cn.com/problems/zui-xiao-tiao-yue-ci-shu) | HARD | 6 | 1 |
| 2020-12-02 06:37 | [#45 跳跃游戏 II](https://leetcode-cn.com/problems/jump-game-ii) | HARD | 3 | 1 |
| 2020-12-01 11:16 | [#34 在排序数组中查找元素的第一个和最后一个位置](https://leetcode-cn.com/problems/find-first-and-last-position-of-element-in-sorted-array) | MEDIUM | 2 | 1 |
| 2020-11-30 14:17 | [#767 重构字符串](https://leetcode-cn.com/problems/reorganize-string) | MEDIUM | 1 | 1 |
| 2020-11-30 07:56 | [#257 二叉树的所有路径](https://leetcode-cn.com/problems/binary-tree-paths) | EASY | 4 | 1 |
| 2020-11-30 06:10 | [#155 最小栈](https://leetcode-cn.com/problems/min-stack) | EASY | 1 | 1 |
| 2020-11-29 16:43 | [#437 路径总和 III](https://leetcode-cn.com/problems/path-sum-iii) | MEDIUM | 1 | 1 |
| 2020-11-29 14:52 | [#951 翻转等价二叉树](https://leetcode-cn.com/problems/flip-equivalent-binary-trees) | MEDIUM | 1 | 1 |
| 2020-11-29 10:40 | [#341 扁平化嵌套列表迭代器](https://leetcode-cn.com/problems/flatten-nested-list-iterator) | MEDIUM | 6 | **3** |
| 2020-11-29 03:37 | [#976 三角形的最大周长](https://leetcode-cn.com/problems/largest-perimeter-triangle) | EASY | 1 | 1 |
| 2020-11-29 03:03 | [#57 插入区间](https://leetcode-cn.com/problems/insert-interval) | MEDIUM | 2 | **2** |
| 2020-11-28 16:30 | [#416 分割等和子集](https://leetcode-cn.com/problems/partition-equal-subset-sum) | MEDIUM | 11 | **2** |
| 2020-11-26 15:24 | [#137 只出现一次的数字 II](https://leetcode-cn.com/problems/single-number-ii) | MEDIUM | 1 | 1 |
| 2020-11-26 12:07 | [#55 跳跃游戏](https://leetcode-cn.com/problems/jump-game) | MEDIUM | 6 | 1 |
| 2020-11-25 16:14 | [#309 最佳买卖股票时机含冷冻期](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown) | MEDIUM | 1 | 1 |
| 2020-11-25 15:58 | [#123 买卖股票的最佳时机 III](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iii) | HARD | 7 | 1 |
| 2020-11-25 04:25 | [#188 买卖股票的最佳时机 IV](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-iv) | HARD | 3 | 1 |
| 2020-11-24 14:20 | [#3 无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters) | MEDIUM | 9 | **2** |
| 2020-11-23 09:54 | [#438 找到字符串中所有字母异位词](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string) | MEDIUM | 2 | 1 |
| 2020-11-23 09:12 | [#567 字符串的排列](https://leetcode-cn.com/problems/permutation-in-string) | MEDIUM | 5 | 1 |
| 2020-11-23 05:25 | [#76 最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring) | HARD | 10 | **2** |
| 2020-11-21 15:31 | [#712 两个字符串的最小ASCII删除和](https://leetcode-cn.com/problems/minimum-ascii-delete-sum-for-two-strings) | MEDIUM | 1 | 1 |
| 2020-11-21 15:05 | [#583 两个字符串的删除操作](https://leetcode-cn.com/problems/delete-operation-for-two-strings) | MEDIUM | 4 | **2** |
| 2020-11-21 14:09 | [#148 排序链表](https://leetcode-cn.com/problems/sort-list) | MEDIUM | 3 | **3** |
| 2020-11-20 12:08 | [#491 递增子序列](https://leetcode-cn.com/problems/increasing-subsequences) | MEDIUM | 7 | 1 |
| 2020-11-20 05:57 | [#147 对链表进行插入排序](https://leetcode-cn.com/problems/insertion-sort-list) | MEDIUM | 1 | 1 |
| 2020-11-19 04:11 | [#391 完美矩形](https://leetcode-cn.com/problems/perfect-rectangle) | HARD | 1 | 1 |
| 2020-11-18 15:41 | [#134 加油站](https://leetcode-cn.com/problems/gas-station) | MEDIUM | 1 | 1 |
| 2020-11-18 15:05 | [#354 俄罗斯套娃信封问题](https://leetcode-cn.com/problems/russian-doll-envelopes) | HARD | 6 | 1 |
| 2020-11-18 13:41 | [#516 最长回文子序列](https://leetcode-cn.com/problems/longest-palindromic-subsequence) | MEDIUM | 1 | 1 |
| 2020-11-17 15:07 | [#1143 最长公共子序列](https://leetcode-cn.com/problems/longest-common-subsequence) | MEDIUM | 2 | 1 |
| 2020-11-16 16:31 | [#剑指 Offer 03 数组中重复的数字](https://leetcode-cn.com/problems/shu-zu-zhong-zhong-fu-de-shu-zi-lcof) | EASY | 1 | 1 |
| 2020-11-16 16:05 | [#239 滑动窗口最大值](https://leetcode-cn.com/problems/sliding-window-maximum) | HARD | 1 | 1 |
| 2020-11-16 09:10 | [#406 根据身高重建队列](https://leetcode-cn.com/problems/queue-reconstruction-by-height) | MEDIUM | 1 | 1 |
| 2020-11-15 15:08 | [#402 移掉K位数字](https://leetcode-cn.com/problems/remove-k-digits) | MEDIUM | 7 | 1 |
| 2020-11-15 06:23 | [#739 每日温度](https://leetcode-cn.com/problems/daily-temperatures) | MEDIUM | 3 | 1 |
| 2020-11-14 11:58 | [#1122 数组的相对排序](https://leetcode-cn.com/problems/relative-sort-array) | EASY | 1 | 1 |
| 2020-11-13 16:56 | [#1118 一月有多少天](https://leetcode-cn.com/problems/number-of-days-in-a-month) | EASY | 3 | 1 |
| 2020-11-13 16:38 | [#503 下一个更大元素 II](https://leetcode-cn.com/problems/next-greater-element-ii) | MEDIUM | 1 | 1 |
| 2020-11-13 14:50 | [#328 奇偶链表](https://leetcode-cn.com/problems/odd-even-linked-list) | MEDIUM | 2 | 1 |
| 2020-11-12 15:41 | [#628 三个数的最大乘积](https://leetcode-cn.com/problems/maximum-product-of-three-numbers) | EASY | 2 | 1 |
| 2020-11-12 13:23 | [#922 按奇偶排序数组 II](https://leetcode-cn.com/problems/sort-array-by-parity-ii) | EASY | 3 | 1 |
| 2020-11-12 12:59 | [#496 下一个更大元素 I](https://leetcode-cn.com/problems/next-greater-element-i) | EASY | 2 | 1 |
| 2020-11-12 04:19 | [#84 柱状图中最大的矩形](https://leetcode-cn.com/problems/largest-rectangle-in-histogram) | HARD | 6 | **2** |
| 2020-11-11 02:58 | [#130 被围绕的区域](https://leetcode-cn.com/problems/surrounded-regions) | MEDIUM | 3 | 1 |
| 2020-11-10 17:35 | [#LCP 18 早餐组合](https://leetcode-cn.com/problems/2vYnGI) | EASY | 5 | 1 |
| 2020-11-09 16:44 | [#973 最接近原点的 K 个点](https://leetcode-cn.com/problems/k-closest-points-to-origin) | MEDIUM | 3 | 1 |
| 2020-11-08 12:20 | [#122 买卖股票的最佳时机 II](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-ii) | EASY | 1 | 1 |
| 2020-11-07 15:54 | [#327 区间和的个数](https://leetcode-cn.com/problems/count-of-range-sum) | HARD | 2 | 1 |
| 2020-11-07 09:22 | [#252 会议室](https://leetcode-cn.com/problems/meeting-rooms) | EASY | 2 | 1 |
| 2020-11-07 08:55 | [#127 单词接龙](https://leetcode-cn.com/problems/word-ladder) | HARD | 2 | **2** |
| 2020-11-07 02:10 | [#1356 根据数字二进制下 1 的数目排序](https://leetcode-cn.com/problems/sort-integers-by-the-number-of-1-bits) | EASY | 3 | **2** |
| 2020-11-03 13:16 | [#941 有效的山脉数组](https://leetcode-cn.com/problems/valid-mountain-array) | EASY | 3 | 1 |
| 2020-11-03 04:28 | [#140 单词拆分 II](https://leetcode-cn.com/problems/word-break-ii) | HARD | 3 | **2** |
| 2020-11-02 15:31 | [#349 两个数组的交集](https://leetcode-cn.com/problems/intersection-of-two-arrays) | EASY | 1 | 1 |
| 2020-11-01 16:58 | [#381 O(1) 时间插入、删除和获取随机元素 - 允许重复](https://leetcode-cn.com/problems/insert-delete-getrandom-o1-duplicates-allowed) | HARD | 8 | **2** |
| 2020-10-30 11:09 | [#463 岛屿的周长](https://leetcode-cn.com/problems/island-perimeter) | EASY | 1 | 1 |
| 2020-10-30 06:30 | [#129 求根到叶子节点数字之和](https://leetcode-cn.com/problems/sum-root-to-leaf-numbers) | MEDIUM | 2 | 1 |
| 2020-10-29 03:58 | [#845 数组中的最长山脉](https://leetcode-cn.com/problems/longest-mountain-in-array) | MEDIUM | 8 | **2** |
| 2020-10-28 17:06 | [#1024 视频拼接](https://leetcode-cn.com/problems/video-stitching) | MEDIUM | 4 | 1 |
| 2020-10-28 09:19 | [#1207 独一无二的出现次数](https://leetcode-cn.com/problems/unique-number-of-occurrences) | EASY | 1 | 1 |
| 2020-10-27 15:32 | [#144 二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal) | MEDIUM | 5 | **2** |
| 2020-10-26 11:50 | [#1365 有多少小于当前数字的数字](https://leetcode-cn.com/problems/how-many-numbers-are-smaller-than-the-current-number) | EASY | 2 | 1 |
| 2020-10-24 02:54 | [#234 回文链表](https://leetcode-cn.com/problems/palindrome-linked-list) | EASY | 6 | **2** |
| 2020-10-24 01:47 | [#206 反转链表](https://leetcode-cn.com/problems/reverse-linked-list) | EASY | 1 | 1 |
| 2020-10-23 13:12 | [#678 有效的括号字符串](https://leetcode-cn.com/problems/valid-parenthesis-string) | MEDIUM | 5 | 1 |
| 2020-10-23 07:06 | [#621 任务调度器](https://leetcode-cn.com/problems/task-scheduler) | MEDIUM | 2 | 1 |
| 2020-10-22 15:20 | [#763 划分字母区间](https://leetcode-cn.com/problems/partition-labels) | MEDIUM | 2 | 1 |
| 2020-10-21 14:58 | [#925 长按键入](https://leetcode-cn.com/problems/long-pressed-name) | EASY | 7 | 1 |
| 2020-10-20 03:18 | [#143 重排链表](https://leetcode-cn.com/problems/reorder-list) | MEDIUM | 3 | 1 |
| 2020-10-20 02:10 | [#543 二叉树的直径](https://leetcode-cn.com/problems/diameter-of-binary-tree) | EASY | 3 | **3** |
| 2020-10-19 12:00 | [#617 合并二叉树](https://leetcode-cn.com/problems/merge-two-binary-trees) | EASY | 4 | 1 |
| 2020-10-19 11:29 | [#844 比较含退格的字符串](https://leetcode-cn.com/problems/backspace-string-compare) | EASY | 1 | 1 |
| 2020-10-18 16:23 | [#19 删除链表的倒数第 N 个结点](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list) | MEDIUM | 3 | 1 |
| 2020-10-17 07:30 | [#52 N皇后 II](https://leetcode-cn.com/problems/n-queens-ii) | HARD | 1 | 1 |
| 2020-10-16 15:15 | [#977 有序数组的平方](https://leetcode-cn.com/problems/squares-of-a-sorted-array) | EASY | 1 | 1 |
| 2020-10-16 14:09 | [#889 根据前序和后序遍历构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-postorder-traversal) | MEDIUM | 1 | 1 |
| 2020-10-15 13:02 | [#410 分割数组的最大值](https://leetcode-cn.com/problems/split-array-largest-sum) | HARD | 4 | 1 |
| 2020-10-14 17:27 | [#572 另一个树的子树](https://leetcode-cn.com/problems/subtree-of-another-tree) | EASY | 2 | 1 |
| 2020-10-14 16:56 | [#101 对称二叉树](https://leetcode-cn.com/problems/symmetric-tree) | EASY | 1 | 1 |
| 2020-10-14 16:21 | [#116 填充每个节点的下一个右侧节点指针](https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node) | MEDIUM | 2 | **2** |
| 2020-10-14 15:37 | [#1002 查找常用字符](https://leetcode-cn.com/problems/find-common-characters) | EASY | 3 | 1 |
| 2020-10-14 14:32 | [#9 回文数](https://leetcode-cn.com/problems/palindrome-number) | EASY | 1 | 1 |
| 2020-10-14 14:26 | [#695 岛屿的最大面积](https://leetcode-cn.com/problems/max-area-of-island) | MEDIUM | 5 | 1 |
| 2020-10-13 14:45 | [#289 生命游戏](https://leetcode-cn.com/problems/game-of-life) | MEDIUM | 1 | 1 |
| 2020-10-13 13:01 | [#75 颜色分类](https://leetcode-cn.com/problems/sort-colors) | MEDIUM | 9 | **2** |
| 2020-10-10 10:35 | [#15 三数之和](https://leetcode-cn.com/problems/3sum) | MEDIUM | 4 | 1 |
| 2020-10-10 09:26 | [#18 四数之和](https://leetcode-cn.com/problems/4sum) | MEDIUM | 3 | **2** |
| 2020-10-09 11:44 | [#141 环形链表](https://leetcode-cn.com/problems/linked-list-cycle) | EASY | 3 | 1 |
| 2020-10-05 09:35 | [#29 两数相除](https://leetcode-cn.com/problems/divide-two-integers) | MEDIUM | 13 | 1 |
| 2020-10-05 07:25 | [#2 两数相加](https://leetcode-cn.com/problems/add-two-numbers) | MEDIUM | 1 | 1 |
| 2020-10-05 05:25 | [#167 两数之和 II - 输入有序数组](https://leetcode-cn.com/problems/two-sum-ii-input-array-is-sorted) | EASY | 2 | 1 |
| 2020-09-28 16:34 | [#114 二叉树展开为链表](https://leetcode-cn.com/problems/flatten-binary-tree-to-linked-list) | MEDIUM | 2 | 1 |
| 2020-09-28 15:18 | [#剑指 Offer 06 从尾到头打印链表](https://leetcode-cn.com/problems/cong-wei-dao-tou-da-yin-lian-biao-lcof) | EASY | 2 | 1 |
| 2020-09-27 15:20 | [#235 二叉搜索树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-search-tree) | EASY | 3 | 1 |
| 2020-09-25 12:50 | [#226 翻转二叉树](https://leetcode-cn.com/problems/invert-binary-tree) | EASY | 1 | 1 |
| 2020-09-25 12:22 | [#106 从中序与后序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal) | MEDIUM | 3 | **3** |
| 2020-09-25 12:08 | [#968 监控二叉树](https://leetcode-cn.com/problems/binary-tree-cameras) | HARD | 8 | **2** |
| 2020-09-23 14:46 | [#1226 哲学家进餐](https://leetcode-cn.com/problems/the-dining-philosophers) | MEDIUM | 5 | 1 |
| 2020-09-22 13:33 | [#295 数据流的中位数](https://leetcode-cn.com/problems/find-median-from-data-stream) | HARD | 1 | 1 |
| 2020-09-22 08:00 | [#654 最大二叉树](https://leetcode-cn.com/problems/maximum-binary-tree) | MEDIUM | 1 | 1 |
| 2020-09-20 16:28 | [#125 验证回文串](https://leetcode-cn.com/problems/valid-palindrome) | EASY | 4 | 1 |
| 2020-09-20 11:02 | [#1411 给 N x 3 网格图涂色的方案数](https://leetcode-cn.com/problems/number-of-ways-to-paint-n-3-grid) | HARD | 3 | 1 |
| 2020-09-20 02:56 | [#LCP 23 魔术排列](https://leetcode-cn.com/problems/er94lq) | MEDIUM | 7 | 1 |
| 2020-09-20 02:06 | [#404 左叶子之和](https://leetcode-cn.com/problems/sum-of-left-leaves) | EASY | 5 | **2** |
| 2020-09-19 04:44 | [#136 只出现一次的数字](https://leetcode-cn.com/problems/single-number) | EASY | 1 | 1 |
| 2020-09-13 15:49 | [#剑指 Offer 07 重建二叉树](https://leetcode-cn.com/problems/zhong-jian-er-cha-shu-lcof) | MEDIUM | 2 | 1 |
| 2020-09-12 14:10 | [#剑指 Offer 05 替换空格](https://leetcode-cn.com/problems/ti-huan-kong-ge-lcof) | EASY | 2 | 1 |
| 2020-09-12 10:34 | [#179 最大数](https://leetcode-cn.com/problems/largest-number) | MEDIUM | 4 | 1 |
| 2020-09-10 15:25 | [#剑指 Offer 64 求1+2+…+n](https://leetcode-cn.com/problems/qiu-12n-lcof) | MEDIUM | 1 | 1 |
| 2020-09-08 03:09 | [#剑指 Offer 52 两个链表的第一个公共节点](https://leetcode-cn.com/problems/liang-ge-lian-biao-de-di-yi-ge-gong-gong-jie-dian-lcof) | EASY | 2 | **2** |
| 2020-09-07 13:54 | [#剑指 Offer 51 数组中的逆序对](https://leetcode-cn.com/problems/shu-zu-zhong-de-ni-xu-dui-lcof) | HARD | 7 | **2** |
| 2020-09-04 05:22 | [#459 重复的子字符串](https://leetcode-cn.com/problems/repeated-substring-pattern) | EASY | 8 | **2** |
| 2020-09-02 14:39 | [#214 最短回文串](https://leetcode-cn.com/problems/shortest-palindrome) | HARD | 8 | **3** |
| 2020-09-01 12:26 | [#1 两数之和](https://leetcode-cn.com/problems/two-sum) | EASY | 13 | **2** |
| 2020-08-31 09:59 | [#292 Nim 游戏](https://leetcode-cn.com/problems/nim-game) | EASY | 1 | 1 |
| 2020-08-30 13:55 | [#557 反转字符串中的单词 III](https://leetcode-cn.com/problems/reverse-words-in-a-string-iii) | EASY | 1 | 1 |
| 2020-08-29 13:02 | [#332 重新安排行程](https://leetcode-cn.com/problems/reconstruct-itinerary) | MEDIUM | 14 | **2** |
| 2020-08-26 16:44 | [#17 电话号码的字母组合](https://leetcode-cn.com/problems/letter-combinations-of-a-phone-number) | MEDIUM | 3 | 1 |
| 2020-08-25 07:21 | [#26 删除排序数组中的重复项](https://leetcode-cn.com/problems/remove-duplicates-from-sorted-array) | EASY | 3 | 1 |
| 2020-08-25 06:21 | [#剑指 Offer 55 - I 二叉树的深度](https://leetcode-cn.com/problems/er-cha-shu-de-shen-du-lcof) | EASY | 1 | 1 |
| 2020-08-21 15:39 | [#剑指 Offer 55 - II 平衡二叉树](https://leetcode-cn.com/problems/ping-heng-er-cha-shu-lcof) | EASY | 6 | 1 |
| 2020-08-21 03:42 | [#647 回文子串](https://leetcode-cn.com/problems/palindromic-substrings) | MEDIUM | 3 | **2** |
| 2020-08-19 11:45 | [#70 爬楼梯](https://leetcode-cn.com/problems/climbing-stairs) | EASY | 1 | 1 |
| 2020-08-18 08:27 | [#109 有序链表转换二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-list-to-binary-search-tree) | MEDIUM | 1 | 1 |
| 2020-08-15 11:55 | [#322 零钱兑换](https://leetcode-cn.com/problems/coin-change) | MEDIUM | 1 | 1 |
| 2020-08-15 08:13 | [#剑指 Offer 66 构建乘积数组](https://leetcode-cn.com/problems/gou-jian-cheng-ji-shu-zu-lcof) | MEDIUM | 4 | 1 |
| 2020-08-14 07:32 | [#剑指 Offer 53 - II 0～n-1中缺失的数字](https://leetcode-cn.com/problems/que-shi-de-shu-zi-lcof) | EASY | 4 | 1 |
| 2020-08-12 12:02 | [#51 N 皇后](https://leetcode-cn.com/problems/n-queens) | HARD | 1 | 1 |
| 2020-08-12 09:03 | [#46 全排列](https://leetcode-cn.com/problems/permutations) | MEDIUM | 1 | 1 |
| 2020-07-31 15:16 | [#4 寻找两个正序数组的中位数](https://leetcode-cn.com/problems/median-of-two-sorted-arrays) | HARD | 4 | 1 |
| 2020-07-26 10:04 | [#97 交错字符串](https://leetcode-cn.com/problems/interleaving-string) | HARD | 2 | 1 |
| 2020-07-23 09:14 | [#剑指 Offer 46 把数字翻译成字符串](https://leetcode-cn.com/problems/ba-shu-zi-fan-yi-cheng-zi-fu-chuan-lcof) | MEDIUM | 1 | 1 |
| 2020-04-08 13:32 | [#剑指 Offer 13 机器人的运动范围](https://leetcode-cn.com/problems/ji-qi-ren-de-yun-dong-fan-wei-lcof) | MEDIUM | 2 | 1 |
| 2020-04-08 12:24 | [#1111 有效括号的嵌套深度](https://leetcode-cn.com/problems/maximum-nesting-depth-of-two-valid-parentheses-strings) | MEDIUM | 1 | 1 |
| 2020-04-08 08:39 | [#94 二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal) | MEDIUM | 3 | 1 |
| 2020-04-01 09:54 | [#145 二叉树的后序遍历](https://leetcode-cn.com/problems/binary-tree-postorder-traversal) | MEDIUM | 1 | 1 |
| 2020-03-26 14:42 | [#面试题 10.09 排序矩阵查找](https://leetcode-cn.com/problems/sorted-matrix-search-lcci) | MEDIUM | 2 | 1 |
| 2020-03-26 05:31 | [#面试题 03.05 栈排序](https://leetcode-cn.com/problems/sort-of-stacks-lcci) | MEDIUM | 4 | 1 |
| 2020-03-25 16:35 | [#1041 困于环中的机器人](https://leetcode-cn.com/problems/robot-bounded-in-circle) | MEDIUM | 5 | 1 |
| 2020-03-25 12:02 | [#面试题 02.05 链表求和](https://leetcode-cn.com/problems/sum-lists-lcci) | MEDIUM | 2 | 1 |
| 2020-03-25 02:27 | [#279 完全平方数](https://leetcode-cn.com/problems/perfect-squares) | MEDIUM | 2 | 1 |
