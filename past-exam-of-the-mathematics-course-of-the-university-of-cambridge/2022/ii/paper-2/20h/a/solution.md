<h1 id="20h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Distinct [prime-power ideals](../../../../../../prime-power-ideal.md) are pairwise [comaximal](../../../../../../comaximal-ideals.md). For comaximal ideals, [product](../../../../../../product-of-ideals.md) equals [intersection](../../../../../../intersection-of-ideals.md), so [induction](../../../../../../mathematical-induction.md) gives

$$
I=P_1^{m_1}\cdots P_k^{m_k}
=P_1^{m_1}\cap\cdots\cap P_k^{m_k}.
$$

The [Chinese remainder theorem](../../../../../../chinese-remainder-theorem.md) therefore gives the ring isomorphism

$$
\mathcal O_K/I\longrightarrow
\prod_i\mathcal O_K/P_i^{m_i}.
$$

The [ideal approximation theorem](../../../../../../ideal-approximation-theorem.md), proved by applying this [Chinese-remainder](../../../../../../chinese-remainder-theorem.md) map one [prime power](../../../../../../prime-power.md) deeper, supplies

$$
\alpha\in I,\qquad
\alpha\notin P_iI\quad(1\leq i\leq k).
$$

Equivalently, $v_{P_i}(\alpha)=m_i$ at every prime dividing $I$.

Since $(\alpha)\subseteq I$, the [fractional ideal](../../../../../../fractional-ideal.md)

$$
I'=(\alpha)I^{-1}
$$

is an [integral ideal](../../../../../../integral-ideal.md) and $II'=(\alpha)$ is a [principal ideal](../../../../../../principal-ideal.md). At every $P_i\mid I$,  
$v_{P_i}(I')=v_{P_i}(\alpha)-m_i=0$, so $I+I'=\mathcal O_K$.

Choose $\beta\in I$ and $\gamma\in I'$ with $\beta+\gamma=1$. Then  
$\alpha,\beta\in I$. For any $x\in I$,

$$
x=x\beta+x\gamma\in(\beta)+II'=(\beta)+(\alpha).
$$

Thus

$$
\boxed{I=(\alpha,\beta)},
$$

so every [ideal](../../../../../../ideal.md) of $\mathcal O_K$ has a [generating set](../../../../../../generating-set-of-an-ideal.md) of two elements.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
