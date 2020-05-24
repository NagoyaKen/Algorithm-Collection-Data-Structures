# Algorithm & Data structure
## For learning and reviewing various algorithms


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
・要素を番号付けして格納している。
・シーケンスはオブジェクトを順番（シーケンシャル）に処理するためのデータ構造
・基本的なシーケンス型は、リスト 、タプル、rangeオブジェクトの３つ

Iterable
反復可能
・for 文の in に書き込めるオブジェクト

Mutable
変更可能な、変わりやすい、無常の、変えられる、
・値を別のオブジェクトに変更可能

Memo
Objects are Python's abstraction for data. All data in a Python program is represented by objects or by relations between objects. (In a sense, and in conformance to Von Neumann's model of a "stored program computer", code is also represented by objects.)
immutable/mutable変数の参照・浅いコピー・深いコピー

## Common Functions for Big-O
|f(n)|Name|
| ------------- | ------------- |
|1|Constant|
|logN|Logarithmic|
|N|Linear|
|NlogN|Log Linear|
|N**2|Quadratic|
|N**3|Cubic|
|2**N|Exponential|



Linear Search(線形探索）
・配列の先頭から順に比較し探索キーデータを探す。

Nこのデータがある場合の探索に必要な比較回数
・最良：　1回
・最悪：　N回
・平均：(n+1)/2回

参考（C言語）
int linear_search(int array[], int n, int key) {
 int i;
 for(i = 0; i < n; i++){
 if(array[i] == key){
 return i;
   }
  }
  return -1;
 }

Binary Search(2分探索）
・整列済みの配列に対して探索を行う
・配列中央の値と探索キーを比較し、
探索キーの値との大小関係を元に探索を進める。

参考
int binary_search(int array[],int num.int key){
int middle,low,high;
low = 0;
high = num -1;
while(low <= high){
middle = (low + high) / 2;
if(key == array[middle]){
return middle;
}
else if(key<array[midddle]){
high = middle -1;
}
else{
low = middle + 1;
}
}
return -1;
}

*lsearch()やbsearch()関数がある


## 計算量
ビッグ・オー記法
・OはOrderの意味
・データの数と実行時間の関係を表現
・アルゴリズムの速度を比較する

Logarithmic time 対数時間 log2N ,Nlog2N
Polynomial time 多項式時間 N**2
Exponential time 指数関数時間 2**nN

## Stack(積み重ねる）
・push
データをスタック頂上に積む操作。
・pop
データをスタック頂上から取り出す操作
・peek
スタック頂上のデータを削除せずにデータ値を見る場合に使われる。
・swap
スタック頂上にあるデータと、その次にあるデータを入れ替える操作。
・デュプリケート
スタック頂上にあるデータを複製し、複製したデータウィ頂上にプッシュする。


## 数式の記法
・Prefix notation(前置記法)
+ 1 2

・Infix notation(中置記法)
7 + 8

・Postfix notation(後置記法)
7 8 +

区切り記号
・前置記法と後置記法では必要だが中期記法では不要



Queue(待ち行列)
・列に並んで待つことを意味する
・基本的なデータ構造の一つ
・Firt in,First Out:FIFO

キューの構造
・末尾 rear
・先頭　front

enqueue
・データをキューの末尾に入れる操作
・挿入、加列

dequeue
・データをキューの先頭から取り出す操作

Queueの配列を使った実装
・Queueは配列や連結リスト等を使って実装
・先頭と末尾の添え字を記録
・キューの溢れ（overflow)のチェック
・キューが空（empty)かチェック


|||
| ------------- | ------------- |
|||
|||
|||

