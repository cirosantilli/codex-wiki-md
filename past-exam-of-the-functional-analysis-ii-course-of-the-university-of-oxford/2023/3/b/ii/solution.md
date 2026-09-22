<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

As in the preceding part, take $T$ to be a [bounded linear operator](../../../../../continuous-linear-operator.md). For $x\in X$, the [Hilbertian basis](../../../../../hilbertian-basis.md) expansion and continuity of $T$ give

$$
Tx=\lim_{N\to\infty}\sum_{k=1}^N\langle x,e_k\rangle Te_k.
$$

The [triangle inequality](../../../../../triangle-inequality.md), the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) for finite sums, and the [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md) give

$$
\begin{aligned}
\left\|\sum_{k=1}^N\langle x,e_k\rangle Te_k\right\|
&\leq\sum_{k=1}^N|\langle x,e_k\rangle|\,\|Te_k\|\\
&\leq\left(\sum_{k=1}^N|\langle x,e_k\rangle|^2\right)^{1/2}
\left(\sum_{k=1}^N\|Te_k\|^2\right)^{1/2}
\leq\|x\|\|T\|_2.
\end{aligned}
$$

Passing to the limit and taking the supremum over the [unit ball](../../../../../unit-ball.md) proves

$$
\boxed{\|T\|\leq\|T\|_2.}
$$

Thus the [Hilbert-Schmidt norm](../../../../../hilbert-schmidt-norm.md) controls the [operator norm](../../../../../operator-norm.md). Without the boundedness interpretation, the nonzero $R$ constructed in the preceding part has zero printed column sum and makes the requested inequality false.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
