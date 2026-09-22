<h1 id="5h/solution">Solution</h1>

↑ **Parent:** [5H](../5h.md)

Against the two pure column strategies, player one's expected payoffs are $L_1(p)=5-2p$ and $L_2(p)=2+(b-2)p$. A [mixed strategy](../../../../../mixed-strategy.md) of the opponent cannot give a smaller expectation than their minimum. The [zero-sum game](../../../../../zero-sum-game.md) optimization is therefore

$$
\boxed{\max_{0\le p\le1}\min\{5-2p,\ 2+(b-2)p\}}.
$$

The first line decreases. If $0<b<2$, the second also decreases, and their minimum is maximized at $p=0$ with value $2$. If $b=2$, the second line is constantly $2$ and the first is at least $3$, so every $p$ is optimal. For $2<b\le3$, the intersection $p=3/b$ lies at or beyond the right endpoint; the minimum increases throughout $[0,1]$ and is maximized at $p=1$ with value $b$. If $b>3$, the intersection lies inside the interval; the minimum increases before it and decreases afterwards. Thus

$$
\boxed{\begin{array}{c|c|c}
b&\text{optimal }p&\text{game value}\\\hline
0<b<2&0&2\\
b=2&\text{any }p\in[0,1]&2\\
2<b\le3&1&b\\
b>3&3/b&5-6/b
\end{array}}.
$$

For the interior case the opponent can equalize row payoffs with first-column probability $(b-2)/b$, confirming the [minimax theorem](../../../../../minimax-theorem.md) value.

## ↑ Ancestors (10)

1. [5H](../5h.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
