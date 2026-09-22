<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For $1\leq j\leq n$, repeated use of the [floor function](../../../../../floor-function.md) identity gives

$$
X_j=2^{-j}\lfloor2^jX_n\rfloor.
$$

Thus the [filtration](../../../../../filtration-probability-theory.md) satisfies $\mathcal F_n=\sigma(X_n)$. Each positive-[probability](../../../../../probability.md) [atom of a sigma-algebra](../../../../../atom-of-a-sigma-algebra.md) here has the form

$$
A_{n,k}=\{k2^{-n}\leq X<(k+1)2^{-n}\},\qquad 0\leq k<2^n,
$$

with [probability](../../../../../probability.md) $2^{-n}$; $\{X=1\}$ is a possible additional [null set](../../../../../null-set.md) atom. Averaging over each [dyadic interval](../../../../../dyadic-interval.md) gives a version

$$
\boxed{\mathbb E[h(X)\mid\mathcal F_n]
=2^n\int_{X_n}^{X_n+2^{-n}}h(u)\,du\quad\text{almost surely}.}
$$

For a globally defined version of the right side, assign any value, for example zero, on $\{X=1\}$.

Indeed, the displayed [random variable](../../../../../random-variable-split.md) is $\mathcal F_n$-[measurable](../../../../../measurability.md) and bounded by $\sup|h|$. On each $A_{n,k}$ its [integral](../../../../../integral-split.md) is

$$
2^{-n}\,2^n\int_{k2^{-n}}^{(k+1)2^{-n}}h(u)\,du
=\mathbb E[h(X)\mathbf1_{A_{n,k}}],
$$

by the [uniform distribution](../../../../../continuous-uniform-distribution.md). Every member of $\mathcal F_n$ is a [union](../../../../../set-union.md) of the displayed [sets](../../../../../set-split.md) and the possible zero-[probability](../../../../../probability.md) atom. Summing these identities therefore verifies the defining [conditional expectation](../../../../../conditional-expectation.md) property on all of $\mathcal F_n$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
