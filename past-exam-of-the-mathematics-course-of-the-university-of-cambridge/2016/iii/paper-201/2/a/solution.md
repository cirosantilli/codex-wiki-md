<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each deterministic $n$, use the nonnegativity and the [martingale](../../../../../../martingale-split.md) property to obtain

$$
\mathbb E\left[M_{n+1}\mathbf1_{\{M_n=0\}}\right]
=\mathbb E\left[\mathbf1_{\{M_n=0\}}\mathbb E[M_{n+1}\mid\mathcal F_n]\right]=0.
$$

A nonnegative random variable with zero [expectation](../../../../../../expected-value.md) is zero almost surely. Hence $M_{n+1}=0$ almost surely on $\{M_n=0\}$. Intersecting these probability-one statements over all $n$ makes them hold simultaneously, and induction gives

$$
\boxed{M_n=0\text{ for every }n\geq T,\quad\text{almost surely}.}
$$

**Zero is absorbing for a nonnegative martingale.** This is the [absorption at zero of a nonnegative martingale](../../../../../../absorption-at-zero-of-a-nonnegative-martingale.md). On $\{T=\infty\}$ the assertion has no finite-time requirement. No unbounded-time use of the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
