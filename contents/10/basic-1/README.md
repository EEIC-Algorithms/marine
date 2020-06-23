# 基本課題#10-a

*以下の課題においては，入出力や問題文で指示がある場合を除き，実装すべき処理において標準ライブラリや問題で指定されていない外部の関数やライブラリ等を使用しないでください．また，課題によってはコードの一部分（コーディング画面の初期コードとは別のコード）があらかじめ与えられている場合があります． その場合，問題文に明記してありますので，指示に従ってください．*

この課題では、`heapq`モジュールを用いても構いません。

### 問題文
\\(N\\)頂点\\(M\\)辺の有向グラフと頂点\\(S\\)が与えられます。
\\(i\\)番目の辺は重みが\\(d_i\\)で、頂点\\(a_i\\)から\\(b_i\\)に移動することができます。
頂点\\(S\\)を始点とし、\\(S\\)から各頂点\\(0,1,2,...N-1\\)について、最短経路上の辺の重みの総和を出力してください。
\\(S\\)からの経路が存在しない場合は`'INF'`と出力してください。

### 制約
- \\(1 \leq N \leq 100000\\)
- \\(0 \leq M \leq 200000\\)
- \\(0 \leq S \leq N-1\\)
- \\(0 \leq a_i,b_i \leq N-1\\)
- \\(a_i \neq b_i\\)
- \\(0 \leq d_i \leq 10000\\)
- 入力中のすべての値は整数である


### 入力
以下の形式で標準入力から与えられる．

---

\\(N \quad M \quad S\\)
\\(a_0 \quad b_0 \quad d_0\\)
\\(a_1 \quad b_1 \quad d_1\\)
:
\\(a_{M-1} \quad b_{M-1} \quad d_{M-1}\\)

---


### 出力
\\(S\\)から各頂点\\(0,1,2,...N-1\\)について、最短経路上の辺の重みの総和を\\(N\\)行に出力してください。
\\(S\\)からの経路が存在しない場合は`'INF'`と出力してください。

### 入力例1
```
4 5 0
0 1 1
0 2 4
1 2 2
2 3 1
1 3 5
```
### 出力例1
```
0
1
3
4
```

### 入力例2
```
4 6 1
0 1 1
0 2 4
2 0 1
1 2 2
3 1 1
3 2 5
```
### 出力例2
```
3
0
2
INF
```