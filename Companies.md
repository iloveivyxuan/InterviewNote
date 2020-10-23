### Grubhub
- test case: unit test / integration test / load test
- DataStructure: Tree
- 简历问 project / work experience
- 技术面考察的是对一个csv文件的简单处理。大概是对文件中的订单排序，文件中每一行包括了订单本身的id，以及该订单上一单的订单id,顺藤摸瓜即可

On campus（2019）:
和别人有冲突怎办
ddl临近工作做不完怎么办
matrix里找单词（比利口的DFS题目简单的多），给一个matrix里全是字母，一个target单词，找target是否出现在matrix里，target只是某一横行 / 一竖列（不会拐弯）
follow up: 如果找多个字母怎么办 / target长度小于matrix.length怎么办

Onsite（2019）:
第一轮：
组员不做事情怎么办
ddl临近工作做不完怎么办
给一组数据饭店有关的数据： eg. 汉堡——>鸡肉汉堡——> m记aa汉堡
                                           ——> k记bb汉堡

                      ——>牛肉汉堡——> m记cc汉堡
                               ——> k记dd汉堡
     要求根据这些数据构造一棵树 {id:name:category:parent} 这里自己得加一个List存child
     基本上写完了，有点小bug，没来得及改时间到了


第二轮：BQ我忘记了
有一个data stream每次出现一个字母，要求匹配target字符串
follow up: 由多个target要匹配怎么做


Behavior Questions:
- technically challenging problems
- which project are you most proud of and why
- 团队中遇到麻烦如何改进
- project 任务量超了怎么做 project management
- 上班之外的兴趣
- 如何合作
- 被批评怎么办
- 有 conflict deadline 怎么办
- team work 有冲突怎么办
- 介绍简历项目
- 简历里提到的技术细节
- 你在合作中有没有遇到过难以get along with的人，你是怎么处理的，结果怎么样
- ddl临近工作做不完怎么办

Coding Challenge：
- https://en.wikipedia.org/wiki/Luhn_algorithm
- 返回一个数组中的 unique values， space and time complexity， Follow up：如何减少 memory complexity
- SQL, 3 个 tables，join and count
- 带权重的 Graph 去掉权重最少的边，变成 Tree
- matrix里找单词（比利口的DFS题目简单的多），给一个matrix里全是字母，一个target单词，找target是否出现在matrix里，target只是某一横行 / 一竖列（不会拐弯）
follow up: 如果找多个字母怎么办 / target长度小于matrix.length怎么办
- 检验输入字符串是否合规，小括号中括号大括号组成，问了有没有别的字符，就说按有的考虑。 follow up design是字符串太大了怎么办，猜了各种分块merge的操作，最后说是存一下就好了==
- LC 347  Top K Frequent Elements

Concept：
- Tell me sth. about Rails framework
- Ruby 各种基本概念
- 如果让你给Rails加一个feature，你加什么
- 什么是REST，有什么好处坏处，有几种操作（GET, PUT。。。）

OnCampue（2018）
- input：binary tree
output：list of list (把每个同一个depth的treenode value 放在同一个sublist里面 最后return the list of all sublists)

-LC 443 变形
Aa2b2c2x -> Aaabbccx

OnCampue（2017）
题：给两个函数read(), setLength()
read()调用一次读取一个char，每次出现更长的palindrome，调用setLength
比如a b a c b b c
第一个a，调用setLength(1)；第二个a，调用setLength(3)；最后一个c，调用setLength(4)
写白板

Oncampus(2018)
第一轮on campus: BQ + SQL + coding (concatenate string, aaabb -> a3b2, abb -> ab2), 问了你熟悉JAVA10吗， 答曰不熟悉，没用过。请解释process和thread的区别，答曰不太知道。然后问synchonization是啥。一开始问SQL可能是因为我简历上面写了SQL


Onsite（2017）
第一轮是coding，题目非常straight forward，写一个substitution cipher。substitution的mapping是前13个字母对应后13个字母。输入一个string input，输出加密之后的result string。follow up就是自己列举各种test cases，然后写一个Unit test。感觉提问内容是看背景+看面试官的，CS科班的会被问怎么parallel然后再拼回来等等更涉及CS基础知识的问题。然后问了一个behavior，“你在合作中有没有遇到过难以get along with的人，你是怎么处理的，结果怎么样”。
第二轮是design，核心部分是设计一个零钱机，input是amount of money，设定币种为US货币（100，20，10，5，2，1，0.25，0.05，0.01），设计一个class，返回怎么用这些币种凑出amount of money。我没有被要求算法最优解，我的面试官直接表示“算法无所谓，别写代码，只设计API”，然后慢慢往里面加feature，后来从make changes逐渐变成了一个vending machine。科班的小伙伴有被问“如果有很多人同时取钱，怎么处理concurrency问题”之类的问题。
Onsite（2018）
 第二轮onsite: BQ + 打印雪花三角（第一行一个*，第二行三个*，第三行五个*，然后给N，请打印出1-N行），然后问了一道merge interval ([1, 5], [5, 6], [8, 9], [10, 11] -> [1, 6], [8, 9], [10, 11])。 这道题没让写代码。就说了想法。
下午的一轮：设计一个数据结构，能用previous record找next record. ) 比如你知道Order 1001前面一单是Order 9997, 知道Order 9997 前面的一单是 Order 1532....然后请设计一个数据结构，能对应上current order 和previous order。注意order number不一定按照顺序排列，也不一定是int. 当时花了好久理解要干嘛，一开始给的是一个数据库的背景，还以为要写SQL。然后花了很久才明白他让我设计数据结构。

我是通过学校career fair拿到面试的，没有店面。第一场在校面试考的题很简单，两道easy难度的题。到了onsite考的题会变难，感觉是刚刚到hard，我的感悟是一定要把数据结构的基础打牢，多练习tree相关的题目。我印象中没有遇到ood，简历也没有怎么问技术，最多谈谈project和work experience吧。19年的数据点，不知道现在怎么样了。

Onsite(2017):
10月份左右投的。第一轮面试12月上旬左右，20分钟聊天式的电面，recruiter面。第二轮技术面，1月上旬，连续两小时的视频面试。一小时coding,一小时design。分别由一个工程师面的。每一轮都先聊一下简历、介绍公司，然后做题，最后问问题。
coding问的前缀树，实现插入和返回所有具有输入的相同前缀的单词，利特口有差不多题。design让设计一个棋盘游戏。

Experience Onsite(2019):
第一轮implementation of HashMap， 第二轮是LC 59
一轮System design， 设计了就是他们现在所有餐厅的列表，和每个餐厅里面的菜单，然后还有就是restaurant owner他们修改菜单和餐厅信息的页面，大概就是从DB design，到service的设计，然后follow up就是Cache，然后还有如果AWS 某个region down了咋办。最后一轮是和Director聊了一些behavior questions，没啥好说的，问了问我最喜欢的工作环境是什么，我就说了反正我不喜欢micro management 的地方，director说除了standup和sprint也没什么management，然后结束了

Experience(2019):
1. Validate parenthesis（贰拾）
1.1 只有小括号，O(1) space 做：记 open parenthesis counter。面试官硬要我优化成这样，说实话这算法不用 oj 跑一遍我真心里没底这对不对
1.2 大括号，中括号，小括号和<>，只能用 stack 了现在

2.1.1 Random number 1~n
2.1.2 Random number 1~n, 最后一个数字 n 的 weight/概率只有其他的1/10。例如1~10，取1~9其中一个数的概率是10/91，取10的概率是1/91
2.2 OOD: Call center, dispatch rules, representitives

3. BQ，test driven development 的各种理解，microservice 的各种理解

4.1 microservice 之间的通信：MQ，HTTP calls
4.2 研究了半天 decouple，loose couple，tight couple 的概念
4.3 TDD 的理解，pro con
4.4 设计 YouTube：很重视 microservice 的划分，尽量 async 用 mq，然后再提一下 cdn 即可
