<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Harris' inequality](../../../../../../harris-inequality.md) states that, for a [product measure](../../../../../../product-measure.md) on $\{0,1\}^n$ with independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) of parameters $p_i\in[0,1]$, [increasing events](../../../../../../increasing-event.md) $E,F$ satisfy

$$
\boxed{\mathbb P(E\cap F)\geq\mathbb P(E)\mathbb P(F).}
$$

In particular, the uniform [probability measure](../../../../../../probability-measure.md) on the [Boolean lattice](../../../../../../boolean-lattice.md) gives $|E\cap F|\geq|E||F|/2^n$. We give a direct [mathematical induction](../../../../../../mathematical-induction.md) proof, so no stronger correlation theorem is assumed.

Prove more generally that $\mathbb E[fg]\geq\mathbb E[f]\mathbb E[g]$ for real coordinatewise increasing [functions](../../../../../../function-split.md) $f,g$ on the finite cube. For $n=0$ both are constant and equality holds. For the inductive step let $p=p_n$, and let $f_j,g_j$ be the restrictions obtained by setting the last coordinate equal to $j\in\{0,1\}$. Write $a_j=\mathbb E[f_j]$, $b_j=\mathbb E[g_j]$, using the [product measure](../../../../../../product-measure.md) on the other coordinates. Monotonicity gives $a_0\leq a_1$, $b_0\leq b_1$. By the inductive hypothesis and [conditional expectation](../../../../../../conditional-expectation.md),

$$
\begin{aligned}
\mathbb E[fg]&\geq(1-p)a_0b_0+pa_1b_1\\
&=((1-p)a_0+pa_1)((1-p)b_0+pb_1)+p(1-p)(a_1-a_0)(b_1-b_0)\\
&\geq\mathbb E[f]\mathbb E[g].
\end{aligned}
$$

The nonnegative correction term also handles $p=0$ and $p=1$. Taking [indicator functions](../../../../../../indicator-function.md) $f=\mathbf1_E$, $g=\mathbf1_F$ proves [Harris' inequality](../../../../../../harris-inequality.md).

For later use, an [increasing event](../../../../../../increasing-event.md) $E$ and a [decreasing event](../../../../../../decreasing-event.md) $G$ have [negative correlation of increasing and decreasing events](../../../../../../negative-correlation-of-increasing-and-decreasing-events.md). The complement $G^c$ is an [increasing event](../../../../../../increasing-event.md), so

$$
\mathbb P(E\cap G)=\mathbb P(E)-\mathbb P(E\cap G^c)\leq\mathbb P(E)(1-\mathbb P(G^c))=\mathbb P(E)\mathbb P(G).
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
