LeetCode 767.

##### Design
1396. Design Underground System
1472. Design Browser History

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

987. Vertical Order Traversal of a Binary Tree
node => coordinates
- DFS
- BFS
- sort list of tuples

314. Binary Tree Vertical Order Traversal
- BFS

1636. Sort Array by Increasing Frequency
```
freqTable = collections.defaultdict(int)
  for num in nums:
  reqTable[num] += 1

import collections
count = collections.Counter(nums)
```
sorted(nums, key=lambda x:(freqTable[x], -x))

451. Sort Characters By Frequency
sorted(string) => []
- Bucket Sort -> O(n)

977. Squares of a Sorted 

821. Shortest Distance to a Character
prev = float('-inf')
prev = float('inf')

450. Delete Node in a BST
BST
- Inorder traversal of BST is an array sorted in the ascending order.

582. Kill Process

387. First Unique Character in a String


##### Backtracking
- Find all combinations
- Backtracking is an algorithm for finding all solutions by exploring all potential candidates. If the solution candidate turns to be not a solution (or at least not the last one), backtracking algorithm discards it by making some changes on the previous step, i.e. backtracks and then try again.
note:
- whether input can include duplicated numbers
- whether output can include duplicated numbers
- does order matters
797. All Paths From Source to Target
39. Combination Sum
40. Combination Sum II
216. Combination Sum III
77. Combinations
784. Letter Case Permutation
78. Subsets (Input are distinct numbers)
90. Subsets II (Input might contain duplicated numbers)

'a'.isalpha()
'a'.lower()
'a'.upper()
subset include []

##### Recursion / DFS


##### Binary Search Tree
98. Validate Binary Search Tree
- each node has lower bound and upper bound

##### Binary Search
34. Find First and Last Position of Element in Sorted Array
74. Search a 2D Matrix

##### Divide and Conquer

##### Sort
sorted('string', key=count.get)
1366. Rank Teams by Votes


##### Heapq / Priority Queue
heapq.heappush(heap, element)
heapq.heappop(heap)
- Can customize __lt__ and __eq__
```
class Word:
    def __init__(self, freq, word):
        self.freq = freq
        self.word = word
    
    def __lt__(self, other):
        if self.freq == other.freq:
            return self.word > other.word
        return self.freq < other.freq
    
    def __eq__(self, other):
        return self.freq == self.freq and self.word == self.word
```
692. Top K Frequent Words
973. K Closest Points to Origin

##### Clarification
upper-case, lower-case



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
