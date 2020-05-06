# Algorithm Collection & Data structure
For learning and reviewing various algorithms


| 型 | オブジェクトの例 |オブジェクトの性質|
| ------------- | ------------- | ------------- |
|int|0,1,-9|||
|float|0.0,-1.5|||
|bool|True,False|||
|NoneType|None||
|str|'','abc'|sequence Iterable|
|tuple|(),(2,),(1,2,'a')|sequence Iterable|
|range|range(0,4)|sequence Iterable|
|list|[],[1],[1,2,'a']|sequence Iterable Mutable|
|set|set(),{2},|Iterable Mutable|
|dict|{1:a,2:b},{}|Iterable Mutable|

*what do sequence iterable Mutable mean?

sequence
連続、続発、(因果的)連鎖、(連続して起こる)結果、ひと続き、(起こる)順序、(同じ組の)続き札、順位札、シークエンス、(数)列
などの意味がある。
・シーケンスはオブジェクトを順番（シーケンシャル）に処理するためのデータ構造
・基本的なシーケンス型は、リスト 、タプル、rangeオブジェクトの３つ

Iterable
反復可能
・for 文の in に書き込めるオブジェクト

Mutable
変更可能な、変わりやすい、無常の、変えられる、
・値を別のオブジェクトに変更可能

小ネタ
Objects are Python's abstraction for data. All data in a Python program is represented by objects or by relations between objects. (In a sense, and in conformance to Von Neumann's model of a "stored program computer", code is also represented by objects.)
immutable/mutable変数の参照・浅いコピー・深いコピー

