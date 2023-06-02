# 实验报告模板

## 小组成员

- 2021131148-汪南 （组长）
- 2021131133-虞子岳
- 2021131136-张佳伟
- 2021131134-陈凯翔
- 2021131146-祝子傑
## 第四课代码

### 代码 commint 地址

https://github.com/Alfrid-n/Cryptocurrency/pull/4/commits/7f37939d79f5887010aee2dac5ad6ef7998be98d

### 代码截图

Block
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-1.png)
BlockChain
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-2.png)
Transaction
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-3.png)
UTXO
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-4.png)
UTXOPool
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-5.png)
utils
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-6.png)
结果
![image](https://github.com/Alfrid-n/Cryptocurrency/blob/lesson4/src/public/4-7.png)
### 主观与讨论题内容
#### 字典树优缺点
字典树（Trie树）是一种用于字符串查找的数据结构，它的优点和缺点如下：
优点：
1.搜索字符串的时间复杂度与字符串长度无关，只与字符串的数量相关，搜索效率非常高。
2.可以方便地实现字符串的前缀匹配，即查找以某个字符串为前缀的所有字符串。
3.可以应用于字符串排序和统计，具有较高的灵活性和可扩展性。
4.实现简单，易于理解和操作。
缺点：
1.对于大量重复的字符串，会浪费大量的存储空间，且内存访问不连续，性能较差。
2.构建字典树的时间复杂度较高，需要遍历所有字符串并插入每个字符，时间复杂度为 O(nm)，其中 n 是字符串数量，m 是字符串的平均长度。
3.在最坏情况下，即所有字符串的公共前缀长度很长时，字典树的深度会变得很大，会造成搜索效率的降低。
4.当字符串集合动态变化时，需要频繁地重建整个字典树，操作复杂度较高。
综上所述，字典树主要适用于大量字符串的匹配和查找，具有高效的搜索效率和灵活的字符操作能力，但也存在较大的空间浪费和构建时间较长的缺点，因此应根据实际情况进行选择。
#### 如何扩展和优化字典树数据结构
字典树是一个非常有用的数据结构，可以用于字符串的匹配和查找。为了更好地利用字典树，可以使用以下方法来扩展和优化它：
1. 压缩字典树（Compressed Trie）：对于具有许多从根节点到某个叶子节点相同前缀的字典树，可以通过将这些相同前缀压缩为一个节点来减小字典树的规模，从而减少存储空间和构建时间。压缩字典树的查询效率和标准字典树相同。
2. 双向字典树（Bidirectional Trie）：标准的字典树只能在一侧进行深度优先搜索，效率较低，而双向字典树可以同时从根节点和叶子节点进行搜索，速度更快。
3. 基数树（Radix Tree）：在字典树中，每个节点包含一个字符或者字符编号，因此需要占用大量空间。而基数树将多个字符或编号组成的字符串作为一个节点处理，从而减少了空间开销。
4. 带权字典树（Ternary Search Tree）：对于需要从多个字符串中查找某个最长公共前缀或者查找最接近的字符串的情况，可以使用带权字典树，每个节点保存该节点所代表的字符串的权重值，在查找时根据权重值确定下一步的搜索方向。
5. 使用缓存：对于使用字典树的一些应用程序，建立字典树的过程比较耗时，可以使用缓存，将构建好的字典树缓存起来，加快查询速度。
总之，扩展和优化字典树数据结构可以提高查询和存储效率，从而使得字典树可以更广泛地应用于实际情况。
- 2021131146 -祝子傑

