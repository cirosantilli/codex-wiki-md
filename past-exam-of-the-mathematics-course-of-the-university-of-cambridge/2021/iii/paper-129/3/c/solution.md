<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $T=1_A*1_A$ and choose

$$
m=\max\{1,\lceil\log(1/\alpha)\rceil\}.
$$

Apply part b with its error parameter replaced by a sufficiently small absolute multiple of $\varepsilon$. This produces a [vector subspace](../../../../../../vector-subspace.md) $V$ of codimension

$$
O(m\varepsilon^{-2})=O(\varepsilon^{-2}\log(1/\alpha))
$$

with the evident harmless modification when $\alpha=1$.

For $t\in V$, $x\in\mathbb F_p^n$, and $q=2m$, [Hölder's inequality](../../../../../../holder-s-inequality.md) gives

$$
\begin{aligned}
|(T*1_A)(x+t)-(T*1_A)(x)|
&\leq\sum_{a\in A}|T(x+t-a)-T(x-a)|\\
&\leq |A|^{1-1/q}\|\tau_tT-T\|_q.
\end{aligned}
$$

Since $\alpha^{-1/q}\leq e^{1/2}$ by the choice of $m$, the bound from part b is at most

$$
\varepsilon |A|^{2-1/q}N^{1/q}
=\varepsilon\alpha^{-1/q}|A|^2
\leq\varepsilon|A|^2
$$

after absorbing the absolute factor into the chosen error parameter. This is the required uniform estimate for $1_A*1_A*1_A$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 129](../../../paper-129-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
