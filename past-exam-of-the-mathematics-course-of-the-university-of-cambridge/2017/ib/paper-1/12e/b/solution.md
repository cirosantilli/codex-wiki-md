<h1 id="12e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $a,b\in\mathbb R^2\setminus T$. If $a=b$, use the constant [path](../../../../../../continuous-path.md). Otherwise consider the countably many lines through $a$ and a point of $T$, and through $b$ and a point of $T$. Choose a line $L$ whose direction is not parallel to any of these lines; such a direction exists because there are uncountably many directions but only a [countable set](../../../../../../countable-set.md) of forbidden ones. Every forbidden line meets $L$ in at most one point. Choose $c\in L$ outside those countably many intersections and outside $\{a,b\}$.

Neither segment $[a,c]$ nor $[c,b]$ meets $T$: a forbidden point on either segment would put $c$ on the corresponding forbidden line. The piecewise linear [path](../../../../../../continuous-path.md)

$$
\gamma(t)=\begin{cases}a+2t(c-a),&0\le t\le1/2,\\c+(2t-1)(b-c),&1/2\le t\le1\end{cases}
$$

lies in the complement. This proves that the [plane minus a countable set is path connected](../../../../../../plane-minus-a-countable-set-is-path-connected.md).

If a [homeomorphism](../../../../../../homeomorphism.md) $h:\mathbb R^2\to\mathbb R$ existed, its restriction after removing a point $a$ would give a [homeomorphism](../../../../../../homeomorphism.md) between $\mathbb R^2\setminus\{a\}$ and $\mathbb R\setminus\{h(a)\}$. The first is a [path-connected space](../../../../../../path-connected-space.md) and therefore [connected](../../../../../../connected-space.md); the second consists of two separated intervals. Since [homeomorphisms](../../../../../../homeomorphism.md) preserve [connectedness](../../../../../../connected-space.md), $\boxed{\mathbb R^2\not\cong\mathbb R}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12E](../../12e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
