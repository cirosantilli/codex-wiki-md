# Three-way equal-sum partition dynamic programming

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

For [positive integer](positive-integer.md) weights of total $S=3h$, store reachable pairs $(x,y)$ of sums assigned to the first two groups after each input [list prefix](prefix-of-a-list.md). The third sum is determined by the processed total minus $x+y$. Assign each new occurrence to one of the three groups using a fresh layer; accept exactly final state $(h,h)$. The transitions are sound by construction and complete by deleting the last occurrence from a valid assignment. The state range is $0\leq x,y\leq h$, giving $O(n(h+1)^2)$ time and $O((h+1)^2)$ rolling space.

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
