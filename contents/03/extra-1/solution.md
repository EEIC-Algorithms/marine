## 解法
回数を決めうった二分探索を用いて解くことができますが、実現不可能な回数が存在することに注意が必要です。
分母がQの倍数となるようにQで割ったあまりを考えることで単調性が成り立つので二分探索をすることができます。

## 計算量
とりうる答えの最大値をAとすると各クエリにつきO(logA)で求めることができます。