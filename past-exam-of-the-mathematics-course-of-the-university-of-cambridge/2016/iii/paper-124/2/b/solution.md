<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First, the [Cramér model](../../../../../../cramer-model.md) has infinitely many successes [almost surely](../../../../../../almost-sure-convergence.md), so every $P_n$ is finite. Indeed, for each fixed $K\ge3$, [independence](../../../../../../independent-random-variables.md) of the [Bernoulli random variables](../../../../../../bernoulli-distribution.md) gives

$$
\mathbb P(U_j=0\text{ for all }K\le j\le M)=\prod_{j=K}^M\left(1-\frac1{\log j}\right)\le\exp\left(-\sum_{j=K}^M\frac1{\log j}\right)\longrightarrow0.
$$

The sum diverges, for example because $1/\log j\ge1/j$ for $j\ge3$. [Continuity from above of a measure](../../../../../../continuity-from-above-of-a-measure.md) and a countable [union bound](../../../../../../boole-s-inequality.md) exclude a final success.

Fix $\epsilon>0$ and put $L_k=\lceil(1+\epsilon)(\log k)^2\rceil$. Let $A_k$ be the event that the whole interval $k+1,\ldots,k+L_k$ consists of failures. By [independence](../../../../../../independent-random-variables.md) and $1-v\le e^{-v}$,

$$
\mathbb P(A_k)\le\exp\left(-\sum_{j=k+1}^{k+L_k}\frac1{\log j}\right)\le\exp\left(-\frac{L_k}{\log(k+L_k)}\right).
$$

Since $L_k=o(k)$, the exponent divided by $\log k$ tends to $-(1+\epsilon)$. Thus $\mathbb P(A_k)\le k^{-1-\epsilon/2}$ for all sufficiently large $k$. The [Borel-Cantelli first lemma](../../../../../../borel-cantelli-first-lemma.md) shows that [almost surely](../../../../../../almost-sure-convergence.md) every sufficiently large such interval contains a success. Taking $k=P_n$ then gives $P_{n+1}-P_n\le L_{P_n}$ for all sufficiently large $n$.

For each fixed $\epsilon$, the [limit superior](../../../../../../limit-superior.md) of the normalized gap is therefore at most $1+\epsilon$ [almost surely](../../../../../../almost-sure-convergence.md). Intersect the probability-one events for $\epsilon=1/r$, $r\in\mathbb N$, to obtain **the [Cramér model prime-gap upper bound](../../../../../../cramer-model-prime-gap-upper-bound.md)**:

$$
\boxed{\mathbb P\left(\limsup_{n\to\infty}\frac{P_{n+1}-P_n}{(\log P_n)^2}\le1\right)=1.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
