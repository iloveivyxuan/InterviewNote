LeetCode 767.

1396. Design Underground System

155. Min Stack
方法一：memorize current minimum with stack

242. Valid Anagram
collections.defaultdict(lambda: 0)
for _, count in table.items():

451. Sort Characters By Frequency
counts = collections.Counter(s)
for letter, freq in counts.most_common():
bucket sort O(n): if we 

509. Fibonacci Number
Recursion + memerization
DP

445. Add Two Numbers II
- Add strings
- Reverse Linked List
- Add Two numbers (linked lists)


### 电面
LeetCode 1029. Two City Scheduling
Greedy Algorithm
| The idea of greedy algorithm is to pick the locally optimal move at each step, that will lead to the globally optimal solution.

follow up 1：让我自己给自己code review。说了更详细的comment和新建类存数据，没多问。
follow up 2：如果数据量巨大无法在本机内存完成排序怎么办。云计算，没问细节。

Syntax:
`sort` customize key
costs.sort(key = lambda x : x[0] - x[1])

竖着的树和解码string


 2轮technical 各做两道题
10/13 第一轮technical第一题题目是 the kth missing number
[4, 5, 7, 9] k=2 return 8
用binary search. 当场写完 run 过tc
第二题就是classic 1dcandy crush就不多说了
结尾当场通知进入下一轮并约了第二天

LeetCode 抚平有孩子的链表

一道是tree vertical order traversal
另一道是alien dictionary的变种（区别就是新的dictionary aphlabet有两个character长度的）

10/14 第二轮techinical

第一题是 leetcode get random number
第二题 是 一个2dmap
123
456
789
大概这样， 给一个数字 有个helper 会return possible next steps (2->3, 4, 1-> 4) 类似这样
问从1开始jump n次有多少不同的path （只需要number of path）
bfs很容易解，但是更好的是 recursion 用memorization 优化
结束直接约了终面

两轮昂校园：1. listnode如果有down和next，写一个flatten method，把down做成next，next做成down的next
2. 字母list，有三个连续一样的就抵消

第二轮，买股票
三个method
buy(company_name, price, volume)
average_cost(company_name)
top_k_average_cost(k)

比如过买google，第一次买了1份2元的，股票升了，第二次买了2份三元的，平均就是(1 * 2 + 2 * 3) / (1 + 2) = 4
