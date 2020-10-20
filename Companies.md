### Grubhub
- test case: unit test / integration test / load test
- DataStructure: Tree
- 简历问 project / work experience
- 技术面考察的是对一个csv文件的简单处理。大概是对文件中的订单排序，文件中每一行包括了订单本身的id，以及该订单上一单的订单id,顺藤摸瓜即可

On campus:
和别人有冲突怎办
ddl临近工作做不完怎么办
matrix里找单词（比利口的DFS题目简单的多），给一个matrix里全是字母，一个target单词，找target是否出现在matrix里，target只是某一横行 / 一竖列（不会拐弯）
follow up: 如果找多个字母怎么办 / target长度小于matrix.length怎么办

Onsite，两轮:
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
