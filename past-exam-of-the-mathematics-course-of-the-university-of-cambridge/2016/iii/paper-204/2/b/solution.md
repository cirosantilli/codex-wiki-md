<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent the [doubly infinite ladder graph](../../../../../../doubly-infinite-ladder-graph.md) by $\mathbb Z\times\{0,1\}$, with horizontal [edges](../../../../../../edge-of-a-graph.md) between successive columns and a vertical rung at each column. An allowed [self-avoiding walk](../../../../../../self-avoiding-walk.md) is coded by a word in $R,V$. Two successive $V$ steps revisit the preceding [graph vertex](../../../../../../vertex-graph-theory.md) and are forbidden. Conversely, every word without consecutive $V$ steps is a [self-avoiding walk](../../../../../../self-avoiding-walk.md): horizontal steps strictly increase the column, and a column is visited vertically at most once. This establishes a [bijection](../../../../../../bijection.md), not merely an upper bound.

For the [directed ladder self-avoiding walk count](../../../../../../directed-ladder-self-avoiding-walk-count.md), $\sigma_0=1$, $\sigma_1=2$, and for $n\geq2$ a word either ends in $R$, or ends in $RV$. Removing that final block gives

$$
\sigma_n=\sigma_{n-1}+\sigma_{n-2},\qquad\boxed{\sigma_n=F_{n+2}}.
$$

Let $\varphi=(1+\sqrt5)/2$ be the [golden ratio](../../../../../../golden-ratio.md), and $\psi=(1-\sqrt5)/2$. The [Binet formula](../../../../../../binet-formula.md) for the [Fibonacci number](../../../../../../fibonacci-number.md) yields

$$
\sigma_n=\frac{\varphi^{n+2}-\psi^{n+2}}{\sqrt5}
=\frac{\varphi^{n+2}}{\sqrt5}\left(1-\left(\frac\psi\varphi\right)^{n+2}\right).
$$

Since $|\psi|<\varphi$, taking $n$th roots gives **$\lim_{n\to\infty}\sigma_n^{1/n}=\varphi$**. This use of the golden-ratio symbol is independent of the connection rate in Question 1.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 204](../../../paper-204-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
